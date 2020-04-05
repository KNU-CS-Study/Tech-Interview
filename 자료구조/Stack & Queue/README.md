# Stack & Queue



## **스택(Stack)**

- 자료의 입력과 출력을 한 곳(방향)으로 제한한 자료구조
- 선형 자료구조의 일종으로 **LIFO(Last In First Out)** : 나중에 들어간 원소가 먼저 나온다.
- 사용하는 함수 
  - **Top(Peek) ** : 스택 포인터, 현재 Stack으로 할당된 공간에 제일 마지막으로 삽입된  데이터가 저장된 위치를 가리키는 요소이다. 
  - **삽입(Push)** : data를 넣는 것.
    - 구현방법 : 현재 Item이 가지고있는 값을 스택의 Top으로 삽입시키고 스택포인터(Top)을 1증가시킨다.
  - **삭제(Pop)** : 데이터를 빼는 것.
    - 구현방법 : Top위치를 -1 해주면 된다.
  - 없는 자료를 뺄려고 했을 때 발생하는 에러를 Stack Underflow
    - 현재 스택 포인터의 위치가 0일때 pop시도시
  - 스택 크기 이상의 자료를 넣을려고 할때 발생하는 에러를 "Stack Overflow"
    - 현재 스택 포인터의 위치가 (스택 사이즈-1) 일때 push시 
- 스택의 구현방법 2가지 
  - 배열 사용
    - 장점 : 상대적으로 빠르다. 구현이 쉽다.
    - 단점 : 데이터의 최대개수가 제한되어있다.
  - 연결리스트 사용
    - 장점 : 데이터의 최대개수가 한정되어 있지 않다.
    - 단점 : 상대적으로 스택보다는 느릴것이다.
- DFS에서 스택을 활용한다.
- 활용 예시 : 함수의 콜스택, 문자열을 역순으로 출력할 때, 연산자 후위표기법, 페이지 뒤로가기, 실행 취소



## **큐(Queue)**

- 자료의 입력과 출력을 한 쪽 끝(front, rear)으로 제한한 자료구조
  - **front** :  **가장 앞 element 바로 앞**을 가리킨다.
  - **rear** : **가장 뒤 element** 를 가리킨다.
- 선형 자료구조의 일종으로 **FIFO(First In First Out)** : 먼저 들어간 원소가 먼저 나온다.
- 종류
  - 선형큐 : 기본적인 큐의 형태, 큐에 빈 메모리가 남아 있어도 꽉 차있는것으로 판단 가능
  - 원형큐 : 선형큐의 문제를 해결, 메모리 공간은 잘 활용하나 배열로 구현되어 있어서 큐의 크기가 제한됨
  - 링크드리스트 큐 : 큐의 크기가 제한이 없고 삽입, 삭제가 편리하다.
  - 우선순위 큐 : 데이터의 우선순위에 따라 우선순위가 높은 데이터부터 꺼내도록 만들어진 큐
    - 일반적으로 **힙으로 구현**한다.
      - 배열로 구현시에는 삽입시 매번 배열에 저장된 모든 데이터와 비교해야해서 **최악의 경우 우선순위가 가장 낮은 데이터 삽입시 다 비교해야되는 경우**가 있다. 또한 삽입 삭제시 매번 밀고 당겨야 될수도 있다.
      - 연결리스트 또한 마찬가지로 매번 비교해야된다.
      - 배열과 연결리스트 모두 데이터가 많아지면 비효율적이다.
    - 데이터를 삽입할 때 우선순위에 따라 정렬하여 삽입한 후, 한쪽 방향에서만 데이터를 꺼내도록 만들면 됨
- 사용하는 함수 
  - add : item을 리스트의 끝부분(rear)에 추가
    - 구현방법 rear+1 에다가 데이터를 추가한뒤 rear를 1증가시킨다.
  - remove : 리스트의 첫번째 항목(front)을 제거
    - front를 1증가시킨다.
    - 이때 front+1 위치에 있는 값을 뽑아둔뒤 증가시키면 반환도 동시에 시킬 수 있다.
- BFS에서는 큐를 활용한다.
- 쓰임새 : 컴퓨터 버퍼에서 주로 사용, 우선순위가 같은 작업 예약(프린터의 인쇄 대기열), 은행업무, 프로세스 관리, 캐시 구현 



## **덱(Deque)**

- 스택과 큐를 합친 형태, 자료의 입력과 출력을 양 쪽 끝에서 가능하게 하는 선형 자료구조
- FIFO와 LIFO 모두 가능
- 특징
  - 크기가 가변적이다.
  - 앞과 뒤에서 삽입과 삭제가 좋다.
  - 중간에 데이터를 삽입하고 삭제하는것은 용이하지가 않다.
  - 원하는 요소에 바로 접근이 가능하다.
  - 스크롤(scroll) : 입력이 한쪽 끝으로만 가능하도록 제한한 덱
  - 셸프(shelf) : 출력이 한쪽 끝으로만 가능하도록 제한한 덱



## **면접 예상 질문**

- 스택으로 큐을 구현할 수 있을까?

  - 두개의 스택을 활용하여 가능하다.
- Stack을 구현할 때, 배열과 연결리스트의 차이
  - 배열 
    - 장점 : 빠른 접근, 구현이 쉽다.
    - 단점 : 최대사이즈가 제한적이다.
  - 연결리스트
    - 장점 : 공간의 제한이 없다.
    - 단점 구현이 어렵다.
- 스택을 활용한 계산기 구현
  1. 중위표기법 - > 후위표기법
  2. 후위표기법  -> 계산.
- 스택(Stack)에 대해 설명하고 예제소스를 구현해봐라
- Circular queue(환형 큐) realloc 하는 방법알기(사이즈 확장).


- 위의 참고

~~~c++
#include   

int *Stack;
int Size;
int Top;   

void InitStack(int aSize){

     Size = aSize;

     Stack = (int*)malloc(Size * sizeof(int));

     Top -= 1;

}

bool Push(int data){

     if (Top < Size - 1){

         Top++;

         Stack[Top] = data;

         return true;

     }else

         return false;

}

int Pop(){

     if (Top >= 0)

         return Stack[Top--];

     else

         return -1;

}

void FreeStack() { free(Stack); }

void main(){

     InitStack(256);

     Push(7);

     Push(0);

     Push(6);

     while (Top != -1)

         printf("%d\n", Pop());

} 
~~~

- 큐(Queue)에 대해 설명하고 예제소스를 구현해보아라

- 위의 참고

~~~c++
#include 

int *Queue;
int QSize;
int head, tail;

void InitQueue(int size){

     QSize = size + 1;

     Queue = (int*)malloc(QSize * sizeof(int));

     head = tail = 0;

}

bool EnQueue(int data){

     if ((tail + 1) % QSize == head)

         return false;

     Queue[tail] = data;

     tail = (tail + 1) % QSize;

     return true;

}

int DeQueue(){

     int data;

     if (head == tail)

         return -1;

     data = Queue[head];

     head = (head + 1) % QSize;

     return data;

}

void FreeQueue() { free(Queue); }

void main(){

     InitQueue(10);

     printf("빈 상태에서 삭제 할 때 = %d\n", DeQueue());

     for (**int** i = 0; i < 10; i++)

         EnQueue(i);

     printf("가득 찬 상태에서 삽입 %s \n", EnQueue(100) ? "성공" : "실패");

     for int i = 0; i < 10; i++)

         printf("%d ", DeQueue());      FreeQueue();

} 
~~~

- 덱(Deque)에 대해 설명하고 예제소스를 구현해보아라

- 위의 참고



### Reference


* https://91ms.tistory.com/3
* https://devuna.tistory.com/22
* https://mygumi.tistory.com/357
* https://milkcaramel66.tistory.com/11
* https://reakwon.tistory.com/30
* https://blessldk.blogspot.com/2015/01/queue.html
* http://www.hanbit.co.kr/channel/category/category_view.html?cms_code=CMS3942847236
* https://blessldk.blogspot.com/2015/01/queue.html

