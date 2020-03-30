# Stack & Queue



## **스택(Stack)**

- 자료의 입력과 출력을 한 곳(방향)으로 제한한 자료구조

- 선형 자료구조의 일종으로 LIFO(Last In First Out) : 나중에 들어간 원소가 먼저 나온다.

- 사용하는 함수 - Push와 Pop, 

- - 없는 자료를 뺄려고 했을 때 발생하는 에러를 Stack Underflow
  - 스택 크기 이상의 자료를 넣을려고 할때 발생하는 에러를 "Stack Overflow"
  - Top / Peek : 제일 최근에 들어간 데이터, 최근의 데이터

- DFS에서 스택을 활용한다.

- 활용 예시 : 함수의 콜스택, 문자열을 역순으로 출력할 때, 연산자 후위표기법, 페이지 뒤로가기, 실행 취소



## **큐(Queue)**

- 자료의 입력과 출력을 한 쪽 끝(front, rear)으로 제한한 자료구조

- 선형 자료구조의 일종으로 FIFO(First In First Out) : 먼저 들어간 원소가 먼저 나온다.

- 종류

- - 선형큐 : 기본적인 큐의 형태, 큐에 빈 메모리가 남아 있어도 꽉 차있는것으로 판단 가능

  - 원형큐 : 선형큐의 문제를 해결, 메모리 공간은 잘 활용하나 배열로 구현되어 있어서 큐의 크기가 제한됨

  - 링크드리스트 큐 : 큐의 크기가 제한이 없고 삽입, 삭제가 편리하다.

  - 우선순위 큐 : 데이터의 우선순위에 따라 우선순위가 높은 데이터부터 꺼내도록 만들어진 큐

  - - 데이터를 삽입할 때 우선순위에 따라 정렬하여 삽입한 후, 한쪽 방향에서만 데이터를 꺼내도록 만들면 됨

- 사용하는 함수 - enQueue, dnQueue 

- BFS에서는 큐를 활용한다.

- 쓰임새 : 컴퓨터 버퍼에서 주로 사용, 우선순위가 같은 작업 예약(프린터의 인쇄 대기열), 은행업무, 프로세스 관리, 캐시 구현 



## **덱(Deque)**

- 스택과 큐를 합친 형태, 자료의 입력과 출력을 양 쪽 끝에서 가능하게 하는 선형 자료구조

- - 스크롤(scroll) : 입력이 한쪽 끝으로만 가능하도록 제한한 덱
  - 셸프(shelf) : 출력이 한쪽 끝으로만 가능하도록 제한한 덱



## **면접 예상 질문**

- 스택으로 큐을 구현할 수 있을까?

- - 두개의 스택을 활용하여 가능하다.

- 스택(Stack)에 대해 설명하고 예제소스를 구현해봐라

- - 위의 참고

**#include **  

**int*** Stack;

**int** Size;

**int** Top;   

**void** InitStack(**int** aSize){

​     Size = aSize;

​     Stack = (**int***)malloc(Size * **sizeof**(**int**));

​     Top -= 1;

}

**bool** Push(**int** data){

​     **if** (Top < Size - 1){

​         Top++;

​         Stack[Top] = data;

​         **return** **true**;

​     }**else**

​         **return** **false**;

}

**int** Pop(){

​     **if** (Top >= 0)

​         **return** Stack[Top--];

​     **else**

​         **return** -1;

}

**void** FreeStack() { free(Stack); }

**void** main(){

​     InitStack(256);

​     Push(7);

​     Push(0);

​     Push(6);

​     **while** (Top != -1)

​         printf("%d\n", Pop());

} 

- 큐(Queue)에 대해 설명하고 예제소스를 구현해보아라

- - 위의 참고

**#include **

**int** *Queue;

**int** QSize;

**int** head, tail;

**void** InitQueue(**int** size){

​     QSize = size + 1;

​     Queue = (**int***)malloc(QSize * **sizeof**(**int**));

​     head = tail = 0;

}

**bool** EnQueue(**int** data){

​     **if** ((tail + 1) % QSize == head)

​         **return** **false**;

​     Queue[tail] = data;

​     tail = (tail + 1) % QSize;

​     **return** **true**;

}

**int** DeQueue(){

​     **int** data;

​     **if** (head == tail)

​         **return** -1;

​     data = Queue[head];

​     head = (head + 1) % QSize;

​     **return** data;

}

**void** FreeQueue() { free(Queue); }

**void** main(){

​     InitQueue(10);

​     printf("빈 상태에서 삭제 할 때 = %d\n", DeQueue());

​     **for** (**int** i = 0; i < 10; i++)

​         EnQueue(i);

​     printf("가득 찬 상태에서 삽입 %s \n", EnQueue(100) ? "성공" : "실패");

​     **for** (**int** i = 0; i < 10; i++)

​         printf("%d ", DeQueue());      FreeQueue();

} 



- 덱(Deque)에 대해 설명하고 예제소스를 구현해보아라

- - 위의 참고

출처

https://91ms.tistory.com/3

https://devuna.tistory.com/22

https://mygumi.tistory.com/357

https://milkcaramel66.tistory.com/11

https://reakwon.tistory.com/30

https://blessldk.blogspot.com/2015/01/queue.html