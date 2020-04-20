# 힙(heap)

### 힙이란?

힙은 최대값 및 최솟값을 찾아내는 연산을 빠르게 하기 위해 고안된 완전이진트리(complete binary tree)를 기본으로 한 자료구조이다. (+ **우선순위 큐**를 만들 때 가장 많이 사용된다)

힙에는 두가지 종류가 있다.

- 부모노드 키값이 자식노드의 키값보다 항상 큰 '최대 힙'
- 부모노드의 키 값이 자식노드보다 항상 작은 '최소 힙'

### 힙의 삽입 과정

![img](https://t1.daumcdn.net/cfile/tistory/217B574551A98BC101)



![img](https://t1.daumcdn.net/cfile/tistory/0358E14251A98C3524)

우선 완전 이진 트리를 유지해야 하므로, 가장 마지막에 원소를 넣고, 필요한 곳 까지 올린다.

### 힙의 삭제 과정

![img](https://t1.daumcdn.net/cfile/tistory/255DB43D51A98F032F)

우선 최소값인 root를 pop()하고, 완전 이진 트리에서 가장 마지막에 있는 값을 root로 올림.

![img](https://t1.daumcdn.net/cfile/tistory/2109A54551A98FE40B)

그리고 left child, right child 중에 더 작은 값과 비교해서 swap한다.

구현상에서는 물리적으로 swap을  계속 하지는 않고, 논리적을 최종 위치를 계산해서 swap 개수를 최소화 한다. 



### 힙정렬

``` c
void heap_sort(element a[], int n){
  int i;
  HeapType h;

  init(&h);

  for(i=0; i<n; i++){
    insert_max_heap(&h, a[i]);
  }

  for(i=(n-1); i>=0; i--){
    a[i] = delete_max_heap(&h);
  }
}
```

힙에 순서대로 넣고 빼면 된다. 힙의 삽입, 삭제가 log(n)이므로 시간 복잡도는 best, worst, average 모두 nlog(n)이다. 

추가로 힙정렬은 unstable하다.

### online인가에 대한 고찰

힙정렬의 7,6,5,4,3,2,1 을 heapsort할때 일단 step1으로 min heap으로 구성 (이 시점까지 데이터가 들어오면 online이 맞다)

그런데 root를 계속 삭제하며 다시 재정렬을 시킬 때 1,2,3 까지 정렬됬는데 (heap에는 4,5,6,7,8 이 있음) 새로운 데이터로 '1'이 들어오면 힙에 넣었다 빼도, 1,2,3,1이 되서 offline이지 않을까??