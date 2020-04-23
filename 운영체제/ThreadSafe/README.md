# 쓰레드 세이프

 ### 쓰레드 세이프란?

멀티 쓰레드 프로그래밍에서 어떤 함수, 변수, 객체가 여러 쓰레드로 부터 동시에 접근이 이루어져도 프로그램의 실행에 문제가 없음을 뜻함.

#### 쓰레드 세이프를 지키기 위한 방법

1. Re-entrancy
   어떤 함수가 한 스레드에 의해 호출되어 실행 중일 때, 다른 스레드가 그 함수를 호출하더라고 그 결과가 각각에게 올바르게 주어져야한다.
2. Thread-local storage
   공유 자원의 사용을 최대한 줄여 각각의 스레드에서만 접근 가능한 저장소들을 사용함으로써 동시 접근을 막음. 이 방식은 동기화 방법과 관련있고 공유상태를 피할 수 없을 때 사용하는 방식이다.
3. Mutual exclusion
   공유 자원을 꼭 사용해야 할 경우 해당 자원의 접근을 세마포어 등의 락으로 통제한다.
4. Atomic operations
   공유 자원에 접근할 때 원자 연산을 이용하거나 '원자적'으로 정의된 접근 방법을 사용함으로써 상호 배제를 구현할 수 있다.

### Critical Section 이란?

각 프로세스는 임계구역 이라고 부르는 코드부분을 가지고 있다.

한 프로세스가 이 임게구역에서 수행하는 동안 다른 프로세스는 들어갈 수 없어야 함.

### Critical Section의 3요소

1.  **mutual exclusion (상호배제)**  : 특정한 프로세스가 임계구역에서 실행되는 동안, 다른 프로세스가 접근 할 수 없다.

2. **progress (진행)** : 임계구역을 사용하지 않고 있다면, 다른 프로세스가 접근할 수 있도록 한다.

3. **bounded waiting(한정된 대기)** : 임계구역 진입 횟수에 한계가 있어서 같은프로세스가 계속 독점해서 사용하지 못하게 한다. 다른 프로세스들이 기아(starvation)에 빠지지 않도록 한다.

### - etc

프로세스는 4가지 구역으로 나뉘어짐.

```c
do{ /********************* 
entry section 
... */ 
/********************* 
critical section 
... */ 
/********************* 
exit section ... */ 
/********************* 
remainder section ... */ } 
while(true)
```



### Peterson's Solution

두가지 변수를 사용함

**int turn;** //누구의 턴인가(i or j)

**boolean flag[2];** i, j 각각이 들어갈 준비가 되면 true, 아니면 false한다.

![img](https://t1.daumcdn.net/cfile/tistory/9968AF495A309FDF22)

1. flag[i]=true; 로 i가 자신이 들어갈 준비가 됨을 알림
2. turn = j; 로 턴을 상대에게 넘겨줌
3. while(flag[j]&&turn==j); 상대턴이고, 상대가 들어갈 의사가 있으면 무제한 대기,
4. 그 후에 자신의 턴이 오면 critical section을 수행하고 flag[i]를 false로 바꾸어서 다른 프로세스가 들어갈 수 있게 한다.

> 한 번에 한 프로세스만 들어갈 수 있어서 mutual exclusion 만족
>
> 임계구역을 사용하지 않고 있다면, 다른 프로세스가 접근 할 수 있게함 progress 만족
>
> 같은 프로세스가 독점해서 사용하지 못하게함 bounded waiting (자신이 들어가고 싶어서 flag[i]=true;를 했음에도 turn은 j에게 먼저 줌으로 각각이 '한정된 대기' 안에 접근 가능)

즉, critical section의 3요소를 만족하는 풀이법.

하지만 busy waiting을 한다는 단점이 있어서, 실제로는 세마포어와 같은 기법을 사용한다.

위 방법이 소프트웨어적인 방법이라면, 아래에서는 하드웨어 기반 동기화 기법에 대해 알아본다.



### **Synchronization Hardware**

- 단일처리기 환경에서는 공유변수가 변경되는 동안에는 인터럽트가 일어나지 않게 해서 간단히 해결할 수 있습니다.

- 하지만, 다중처리기 환경에서는 이 방법을 적용시킬수 없습니다. 모든 처리기에 인터럽트를 하지 못하게 메시지를 전달하기엔 CPU의 이용률은 떨어뜨리기 때문입니다.



### Atomic Operation = 인터럽트 되지 않는 하나의 단위를 가진 명령어

1. **test_and_set() **

```java
boolean test_and_set(boolean *target) 
{ 
    boolean rv = *target; 
    *target = true; 
	return rv; 
}
```

- 인자로 받은 변수(target)를 true로 하고, return은 원래의 target값이다.

```c
do{ 
    while(test_and_set(&lock)) 
        /*do nothing*/ ; 
    /********************* 
    critical section */ 
    lock = false; 
    /********************* 
    remainder section */ 
} while(true);

출처: https://hongku.tistory.com/17?category=800115 [IT에 취.하.개.]
```



- 자기가 들어가면서 문을 잠그는 느낌. (false일 때, false를 맅너해서 while문을 한번에 통과할 수 있고 값 자체는 이제 true가 되어서 다른 프로세스는 통과 못함)



2. **compare_and_swap()**

```c
int compare_and_swap(int *value, int expected, int new_value)
{ int temp = *value; 
 if(*value = expected){ 
     *value = new_value; 
 } 
 return temp; 
}

```

```c
do { 
    while(compare_and_swap(&lock, 0, 1) != 0) 
        /* do nothing */ 
        ; /********************* 
        critical section */ 
    lock = 0; 
    /********************* 
    remainder section */ 
} while(true);

```

- 비슷하게 0을 가지고 있으면, 1을 로 바꾸고 리턴은 0으로 한다.
- 1을 가지고 있으면 계속 1을 리턴한다.



- 이도 비슷하게 자기가 들어가면서 문을 잠그는 느낌이다. 자신이 0이면 통과하면서 값 자체는 1로 바꿔서 다른 프로세스가 들어오지 못하게 한다. 



### Mutex Lock (뮤텍스 락)

하지만 하드웨어 동기화는 응용프로그래머가 사용할 수 없는 방법이기 때문에, 운영체제 설계자들이 개발해 준 도구가 mutex lock임.

mutex는 mutial exclusion의 줄임말임.

![img](https://t1.daumcdn.net/cfile/tistory/9949BC485A30D9132E)

>  test_and_set()과 비슷하게  사용 가능.

지금까지 설명한 구현 방법은 Busy Waiting (바쁜 대기)을 해야한다는 것입니다. 임계구역에 들어가기 위해서 계속 while()문에서 대기해야 합니다. 이런 busy waiting은 CPU cycle을 낭비하게 됩니다.

프로세스가 계속 반복 회전하고 있기 때문에 spinlock이라고 부르기도 합니다.



mutex lock이랑 비슷하지만, 보다 정교하게 동기화 할 수 있는 Semaphore에 대해 알아보겠습니다.

### Semapohre (세마포어)

운영체제에서는 종종 카운팅 세마포어, 이진 세마포어를 구분합니다. 여기서 이진 세마포어는 0과 1를 가지고 동작하고, mutex lock과 유사하게 동작합니다.

mutex와 가장 큰 차이점은  **관리하는 동기화 대상이 갯수입니다  **Mutex는 동기화 대상이 오직 하나뿐일 때,**Semaphore는 동기화 대상이 하나 이상일 때 사용합니다.**

![img](https://t1.daumcdn.net/cfile/tistory/99131C395A30DB5107)



semaphore 접근 함수는 wait(), signal()이 있다.   wait()는 사용할 때 -1 해주고 signal()은 반납할 때 +1 해준다. 이 둘 함수를 조합하여서 사용하며, semaphore의 초기값이 n이라면, 최대 n개의 프로세스 까지 공유자원을 동시에 사용 가능하다.



### References

* [https://gompangs.tistory.com/entry/OS-Thread-Safe%EB%9E%80](https://gompangs.tistory.com/entry/OS-Thread-Safe란)

  