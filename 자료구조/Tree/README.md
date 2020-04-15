# Tree

## 트리란 

트리는 **node(노드)와 edge로 이루어진 자료구조**이며 싸이클을 가지지 않는 자료구조이다.

1. 트리는 하나의 루트 노드를 갖는다.
2. 루트 노드는 0개 이상의 자식 노드를 갖고 있다.
3. 그 자식 노드 또한 0개 이상의 자식 노드를 갖고 있고, 이는 반복적으로 정의된다.
4. 그래프의 한 종류이다.
5. 트리에는 사이클이 존재할 수 없다.
6. 비선형 자료구조로 계층적 관계를 표현한다.
7. 트리는 이진 트리, 이진 탐색 트리, 균형 트리(AVL 트리, red-black 트리), 이진 힙(최대힙, 최소힙) 등이 있다.

#### 트리 용어

* **node** : 트리는 노드들의 집합으로 트리를 구성한다. 보통 값과 부모 자식 정보를 가지고 있다.
* **root node** : 가장 상위 노드로 부모를 가지지 않는다.
* **leaf node** : 가장 하위 노드로 자식을 가지지 않는다.
* **Sibilings(형제노드)** : 같은 부모를 가지는 자식 노드들을 말한다.
* **depth** : tree에서 부모에서 자식순으로 이동할때, depth가 1 증가하며 따라서 형제 노드 간에는 depth가 일치하며 root node 의 경우에는 depth가 0이 된다.
* **degree of a node (노드의 degree)** : 노드의 degree는 subtree의 개수라고 보면된다.
* **degree of a tree (트리의 degree)** : 그 트리에 있는 노드들중 최대 degree.
* **level of a node** : root가 1로 생각하고 계산하면 된다.



#### 트리가 사용되는 곳

리눅스와 윈도우 같은 운영체제의 파일 시스템들은 모두 트리를 이용해서 만듭니다. 

아래는 윈도우 파일 시스템 파일 구조입니다.

![image](https://user-images.githubusercontent.com/36303777/77856369-9fe88080-7231-11ea-8c7d-fbe9f8bbe01a.png)

그림 출처-[www.co-bw.com](http://www.co-bw.com/DMS_file_management.htm)



### 트리와 그래프의 차이

![img](https://gmlwjd9405.github.io/images/data-structure-graph/graph-vs-tree.png)

사진 출처 : https://gmlwjd9405.github.io/2018/08/12/data-structure-tree.html



## 트리의 종류

>  트리는 우선 가장 크게 **Binary Tree**와 **Non-Binary Tree**로 나뉩니다.

### Non-Binary Tree


binary tree가 아닌 트리.

### Binary Tree(이진트리)

> 정의 - 이진트리는 공백이거나 루트와 왼쪽서브트리, 오른쪽 서브트리라고 하는 2개의 분리된 이진트리로 구성된 노드의 유한집합이다. 

* 각 노드의 차수가 2를 넘지않는다. 즉, 각 노드의 child(자식)의 개수가 2개이하이다.
* 왼쪽 서브트리와 오른쪽 서브트리를 구분한다.
* 0개의 노드를 가질 수 있다.

#### 특이한 Binary Tree 들

##### **Skewed Binary Tree**

한방향으로 편향된 Binary Tree 이다.

<img src="https://user-images.githubusercontent.com/36303777/77856632-6b75c400-7233-11ea-823e-0dd739fd465c.png" alt="image" style="zoom: 50%;" />

##### **Complete Binary Tree**

depth가 가장 낮은 tree이다. 가장 최적화된 tree이고 **depth가 낮아서 search할때 유리하다.**

<img src="https://user-images.githubusercontent.com/36303777/77856628-69136a00-7233-11ea-8d34-50d3bf80857a.png" alt="image" style="zoom:50%;" />

##### **Full Binary Tree**

tree가  꽉찬 경우이다.


$$
depth 가   k일 때 :
node의 개수는 2^k-1
$$


![image](https://user-images.githubusercontent.com/36303777/77856719-0b335200-7234-11ea-96a6-191454c487a3.png)



#### 배열로 표현한다면 ?

root 는 1번째 index에 위치

왼쪽 자식은 x2

오른쪽자식은 x2+1

부모는 /2  해주면된다.

![image](https://user-images.githubusercontent.com/36303777/77856876-2488ce00-7235-11ea-9b8e-123cf1ee14cc.png)




#### Binary Tree의 순회방법 3가지

* **inorder (중위순회)**

  * left -> print ->right 순

  * ~~~c++
    void inorder(treePointer ptr){
        if(ptr){
            inorder(ptr->leftChild);
            printf("%d",ptr->data);
            inorder(ptr->rightChild);
        }
    }
    ~~~

  * 호출순서<img src="https://user-images.githubusercontent.com/36303777/77857195-12a82a80-7237-11ea-980f-158ba02bf8f5.png" alt="image" style="zoom:50%;" />

    

* **preorder(전위순회)**

  * print -> left -> right 순

  * ~~~c++
    void preorder(treePointer ptr){
        if(ptr){
            printf("%d",ptr->data);
            preorder(ptr->leftChild);
            preorder(ptr->rightChild);
        }
    }
    ~~~

  * 호출순서<img src="https://user-images.githubusercontent.com/36303777/77857217-2bb0db80-7237-11ea-9e1c-377e30976493.png" alt="image" style="zoom:50%;" />

* **postorder(후위순회)**

  * left->right -> print 순

  * ~~~c++
    void postorder(treePointer ptr){
        if(ptr){
            postorder(ptr->leftChild);
            postorder(ptr->rightChild);
            printf("%d",ptr->data);
        }
    }
    ~~~

  * 호출순서<img src="https://user-images.githubusercontent.com/36303777/77857222-2e133580-7237-11ea-854f-a2bad58ff276.png" alt="image" style="zoom:50%;" />

* 추가적으로 **level order**가 있는 데 왼쪽 위부터 차례대로(level대로 출력) BFS하듯이 순서대로 탐색하는 방식이다.
  
  * queue를 통하여 구현한다.

## Heap

우선순위 큐를 구현하는데 주로 사용된다. 우선순위를 가지고 있고 젤 큰값(**Max Heap**) 혹은 젤 작은값(**Min Heap**)을 뽑아올 수 있다. 

> Heap 에 관해서는 추후자세히 정리할 예정이다.



## Binary Search Tree

> 효율적인 탐색이 가능한 트리. 이진트리의 일종.

BST 에는 **데이터를 저장하는 규칙**이 있다.

1. 이진 탐색 트리의 노드에 저장된 키는 유일하다.
2. 루트 노드의 키가 왼쪽 서브 트리를 구성하는 어떠한 노드의 키보다 크다.
3. 루트 노드의 키가 오른쪽 서브 트리를 구성하는 어떠한 노드의 키보다 작다.
4. 왼쪽과 오른쪽 서브트리도 이진 탐색 트리이다.



* BST 탐색 연산의 시간복잡도 : O(log n)

* **문제점** : [skewed Tree(편향 트리)](#####**Skewed Binary Tree**)인 경우에 저장순서에 따라 계속 한쪽으로만 노드가 추가되는데 이럴 경우에는 worst case로써 시간복잡도가 O(n)이다.

* **해결방안** : `Rebalancing 기법`을 적용한다. 균형을 잡기위한 트리 구조의 재조정을 Rebalancing 이라고 하는데 그중 유명한 것이 `Red-Black Tree `이다.(이부분에 대해선 추후에 다룰 예정이다.)


## 면접 질문

### 1. BST(Binary Search Tree)에서 원하는 데이터를 탐색할 때 시간 복잡도를 구하라.

- 일반적인 경우의 시간은 **O(log N)** 시간이 걸린다.
- 그러나 **편향트리(skewed binary tree)의 경우**, 시간은 **O(N)** 시간이 걸린다.
  - 이를 해결하기 위해서 **트리 구조의 재조정(Rebalancing)**을 진행한다.
  - 대표적인 트리로  Red-Black tree가 있다.



### 2. 트리와 그래프의 차이

* 그래프
  * 방향 : 방향이 있을 수도 없을 수도 있다.
  * 사이클 : 사이클이 존재할 수도 있다.
  * 루트노드나 부모, 자식 개념이 없음
* 트리
  * 방향 : 방향이 항상 존재한다.
  * 사이클 : 사이클이 발생하지 않는다.
  * 한개의 루트노드, 부모 자식개념이 존재

### 3. 2018 카카오 필기문제

![image](https://user-images.githubusercontent.com/41226017/79304594-aadb2a80-7f2c-11ea-918e-088d0c749ed5.png)


Reference

* [http://www.secmem.org/blog/2019/05/09/%ED%8A%B8%EB%A6%AC%EC%9D%98-%EC%A2%85%EB%A5%98%EC%99%80-%EC%9D%B4%ED%95%B4/](http://www.secmem.org/blog/2019/05/09/트리의-종류와-이해/)
* https://gmlwjd9405.github.io/2018/08/12/data-structure-tree.html
