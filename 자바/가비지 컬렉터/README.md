# Garbage Collector (가비지 컬렉터)




## 가비지(Garbage)란?

* 정리되지 않은 메모리
* 유효하지 않은 메모리 주소.

~~~java
int[] array = new int[3];

array[0] = 1;
array[1] = 10;
array[2] = 20;

//새로운 String 타입의 배열을 만들어서 array가 새로운 배열을 가리키게함.
array = new String{'가','나','다','라','마'};
~~~

이때 기존의 array 가 가리키고 있던 int타입의 3칸짜리 배열은 주소를 잃어버려서 사용할수 없는 메모리가 된다.(정리되지 않은 메모리)

이를 자바에서는 **가비지(Garbage)**라고 부른다.


다른 예시

~~~java
public class Garbage {
    public static void main(String[] args) {
        String str = "asdf";
        str += "qwer";
        System.out.println(str);
    }
}
~~~

![image](https://user-images.githubusercontent.com/36303777/79490892-8bd9b700-8058-11ea-880c-dc1095f90568.png)

문자열 더하기 연산이 수행되는 과정에서(String은 불변객체 이므로) 기존에 있던 "asdf"스트링에 "qwer"을 덧붙이는 것이 아니라, 문자열에 대한 더하기 연산이 수행된 결과가 새롭게 heap영역에 할당된다.


## 가비지 컬렉터란?

>가비지 객체의 메모리를 해제시킨다.

**쓰레기 객체를 효과적으로 처리하는 작업을 GC** 라고 합니다.
JVM의 가비지 컬렉터는 정리되지 않은 채로 남겨져 있는 메모리들을 다른용도로 사용할 수 있게 **메모리 해제**를 시키는 프로그램이다.



### GC 과정

GC의 과정을 `Mark and Sweep`이라고도 한다. GC가 스택의 모든 변수 또는 Reachable 객체를 스캔하면서 각각 어떤 객체를 참조하고 있는지 찾는 과정이 **Mark** 라고 한다. 이 과정에서 Stop the world가 발생한다. 이후 Mark 되어있지 않은 객체들을 힙에서 제거하는 과정이 **Sweep** 이다.

> **Stop the world**는 GC 실행을 위해 JVM이 애플리케이션 실행을 멈추는 것이다.

> JVM의 Heap은 Young, Old, Perm 세 영역으로 나뉜다. Young 영역에서 발생(새롭게 생성된 객체가 존재)하는 GC를 **Minor GC**이라 하고 나머지 두영역(Old - reachable 상태를 유지해 살아남은 객체가 존재, Perm - 거의 사용되지 않음)에서 발생한 GC를 **Major GC**이라 한다. 




## 가비지 컬렉터가 실행되는 시점.

> 메모리를 더 달라고 요청하는 때에 실행.

JVM은 메모리를 부여받고 열심히 프로그램들을 실행하다가 메모리가 부족해지는 순간이 오면 OS에게 추가로 메모리를 더 요청하게 된다.
이 시점에서 가비지 컬렉터(Garbage Collector)가 실행된다.



## Reachability

Java의 GC는 가비지 객체를 판별하기 위해 **reachability** 라는 개념을 사용한다. 어떤 객체에 유효한 참조가 있으면 'reachable', 없으면 'unreachable'로 구별하고 'unreachable'객체를 가비지로 간주한다.

> reachability를 제어할 수 있다면 코드를 통해 Java GC에 일부 관여할 수 있다.








## Reference

* JAVA::가비지컬렉터란 : [https://wanzargen.tistory.com/15](https://wanzargen.tistory.com/15)
* 성능튜닝 가비지 컬렉터 이해하기 : [https://12bme.tistory.com/57](https://12bme.tistory.com/57)
* 자바 메모리 관리 - 가비지 컬렉션 : [https://yaboong.github.io/java/2018/06/09/java-garbage-collection/](https://yaboong.github.io/java/2018/06/09/java-garbage-collection/)
* 가비지 컬렉터 GC - [https://velog.io/@litien/%EA%B0%80%EB%B9%84%EC%A7%80-%EC%BB%AC%EB%A0%89%ED%84%B0GC](https://velog.io/@litien/가비지-컬렉터GC)

