### BST

- 각 노드에 값이 있다.
- 노드의 왼쪽 서브트리에는 그 노드의 값보다 작은 값들을 지닌 노드들로 이루어져 있다.
- 노드의 오른쪽 서브트리에는 그 노드의 값과 같거나 큰 값들을 지닌 노드들로 이루어져 있다.
- 좌우 하위 트리는 각각이 다시 이진 탐색 트리여야 한다.
- 중위 순회(inorder traversal)를 하게 되면 오름차순으로 정렬된 key값을 얻을 수 있다.

- 보통 탐색의 경우 log(n)시간이 걸리지만, 트리가 편향된(skewed) 경우, N타임이 걸리기 때문에, 편향성을 방지하기 위해 AVL트리 or Red Black 트리를 사용한다

-->Blanced Binary Tree --> (AVL, Red Black)

### AVL 트리

- AVL트리에서 노드의 두 하위 트리(왼쪽, 오른쪽)의 높이 차이가 최대 1을 넘지 않는다

- **엄격하게 균형을 유지해서 red-black 트리보다 더 빠르지만, 더 많은 작업을 수행해야만 한다.**

- 대부분의 연산은 이진탐색트리와 동일하다

- 모든 노드는 최대 2개의 자식노드를 가질 수 있고, 왼쪽 자식노드는 부모보다 작고, 오른쪽 자식노드는 부모모도 크다.

- 모든 삽입, 삭제, 탐색 연산에서 **트리가 균형을 가지는지 확인**

- 삽입, 삭제, 탐색 연산에서 평균복잡도, 최악 복잡도 모두 O(logN)

- height를 기준으로 LL, LR, RL, RR을 판단하고, 회전을 통해서 균형을 유지

  

### 구현방법

자세한 구현방법은 https://doublesprogramming.tistory.com/237 참고



### Red Black Tree

- [자가 균형 이진 탐색 트리](https://ko.wikipedia.org/wiki/자가_균형_이진_탐색_트리)
- 트리에 n개의 원소가 있을 때 [O](https://ko.wikipedia.org/wiki/점근_표기법)(log *n*)의 시간복잡도로 삽입, 삭제, 검색을 할 수 있다.

- AVL트리보다는 덜 엄격하다
- 모든 삽입, 삭제, 탐색 연산에서 **트리가 균형을 가지는지 확인**

- Red, Black으로 트리의 균형을 유지

  ### RedBlack Tree Rule

  - 모든 노드는 RED이거나 BLACK이다.
  - 루트는 BLACK이다.
  - 모든 리프(NIL)는 BLACK이다.
  - 노드가 RED이면 그 노드의 자식은 모두 BLACK이다. // NO Double Red
  - 각 노드로부터 그 노드의 자손인 리프로 가는 경로들은 모두 같은 수의 BLACK 노드를 포함한다.



### 구현방법

자세한 구현방법은 https://nesoy.github.io/articles/2018-08/Algorithm-RedblackTree 참고



### RedBlack과 AVL의 차이점

- AVL Tree가 Red Black Tree보다 빠른 Search를 제공합니다.
  - AVL Tree가 더 엄격한 Balanced를 유지하고 있기 때문입니다.
- Red Black Tree은 AVL Tree보다 빠른 삽입과 제거를 제공합니다.
  - AVL Tree보다 Balanced를 느슨하게 유지하고 있기 때문입니다.
- Red Black Tree는 AVL Tree보다 색깔을 저장하기 위해 더 많은 Space Complexity가 필요합니다. (O(n)인건 같다)
- Red Black Trees는 대부분의 언어의 map, multimap, multiset에서 사용하고 있습니다.
- AVL tree는 조회에 속도가 중요한 Database에서 사용하고 있습니다.

### RedBlack Tree 복잡도(Complexity)에 대해

| Algorithm | Average  | Worst case |
| :-------- | :------- | :--------- |
| Space     | O(n)     | O(n)       |
| Search    | O(log n) | O(log n)   |
| Insert    | O(log n) | O(log n)   |
| Delete    | O(log n) | O(log n)   |





### Reference 

[https://ko.wikipedia.org/wiki/%EC%9D%B4%EC%A7%84_%ED%83%90%EC%83%89_%ED%8A%B8%EB%A6%AC](https://ko.wikipedia.org/wiki/이진_탐색_트리)

https://doublesprogramming.tistory.com/237

https://nesoy.github.io/articles/2018-08/Algorithm-RedblackTree

