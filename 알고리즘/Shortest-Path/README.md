# 최소 경로 알고리즘들 비교

1. 벨만 포드
2. 다익스트라
3. Floyd-Washall
4. BFS (간선간의 weight가 없을 때 사용)



### 유형에 따른 구분

1. Single-source : 하나의 출발 노드 s로 부터 다른 모든 노드까지의 최단 경로를 찾아라 (**Dijkstra, 벨만 포드 알고리즘**)

2. Single-destination :  모든 출발 노드로부터 하나의 목적지 노드 까지의 최단 경로를 찾아라 //**무방향 그래프이면 single-source 문제와 같다**

3. Singe-pair : 하나의 출발 노드 -> 하나의 목적적지 노드 // **worst case가 single-source보다 항상 나쁘다.** but 가장 효율성, 실용성 있는 문제

4. All-paris : 모든 노드 쌍에 대해서 최단 경로를 찾아라 (**플로이드 알고리즘**)



### 짚고 넘어갈 것

1. 음수 가중치 // 거리가 음수인 경우. 많은 알고리즘에서 없다고 가정하지만, '음수 가중치' 자체는 **존재하는 경우도 있다.**
2. 음수 사이클 // 모든 경로의 합, 길이가 음수가 나오는 것. 사이클이 돌면 돌수록 길이가 짧아지므로 현실적으로 말이 되지 않는다. 따라서 **음수 사이클이 있으면 최단 경로**가 정의되지 않는다.

3. **최단 경로는 모든 최단 경로들의 합**이다. (Greedy 하게 접근 가능)

4. 기본적으로 Relaxtion 연산으로 경로를 찾는다.

   #### Relaxtion이란 ?

   ![img](https://t1.daumcdn.net/cfile/tistory/2144094A5931610B2A)

1. 간단히 설명하자면, a->b로 가는 것이 빠른지 'c' 를 거쳐서 a->c->b로 가는 것이 빠른지를 비교하며 진행하는 연산이다.
2. 알고리즘들 간의 차이는 relax연산을 어떤 엣지에 대해서, 어떤 순서로 하느냐에 따라서 발생한다.

### 벨만 포드 알고리즘

1. 방향 그래프에서 사용
2. 음의 가중치를 가지는 그래프에서 사용 가능
3. Single source--> All Destination
4. Greedy 하지 않다(완전 탐색에 가깝다) --> 모든 경우의 수 탐색
5. 음의 싸이클이 있으면, 탐색이 최단경로를 못찾지만, **음의 싸이클의 존재 유무 자체는 알 수 있다.**



#### concept

그래프 내 모든 엣지에 대해 edge relaxation을 수행 ==> (|V|−1)회 수행하게 된다. 

![img](https://i.imgur.com/hcWT22F.png)

- 음수 가중치를 가지고 있어도 작동 가능

- **음수 싸이클**을 가지고 있으면 **최단경로를 찾지 못한다.**

  

  ex) ![img](https://i.imgur.com/46tJqd7.png)

[참고자료] : 음수 싸이클을 가지는 그래프, [e, f]구간을 돌면 그 거리가 계속 작아져 최단 경로가 의미없게 된다. [c1,d]구간은 싸이클일 돌수록 거리가 커져서 문제가 되지 않음

- 하지만 **음수 싸이클**이 있는지 없는지 알 수 있다!

  #### 어떻게?

  "정상적인 그래프라면, 즉, 음의 사이클이 발생하지 않는 그래프라면, N - 1번을 탐색한 이후에, 또 한번의 탐색을 더 하더라도 절대로 ! 최소비용이 변하는 정점이 발생하지 않는다"

  라는 사실을 이용한다.

  



#### 계산복잡성

- 모든 엣지에 대해, 전체 노드 수 만큼 반복해주므로 O(VE)가 된다. 

- 그런데 dense graph는 엣지의 수가 노드 수의 제곱이 되므로 O(V^3)에 가깝다.

- 다익스트라의 O(V^2)에 비해 느리지만, **음수인 가중치도 가능하다는 장점**이 있다.



### 다익스트라 알고리즘

1. singlue source, one destination

2. 음수 싸이클, 음수 가중치가 없는 그래프에서 사용

3. 이를 확장시킨 알고리즘이 A* 알고리즘이다.

   #### A* 알고리즘 이란?

   현재 상태의 비용을 g(x)*g*(*x*), 현재 상태에서 다음 상태로 이동할 때의 [휴리스틱](https://namu.wiki/w/휴리스틱) 함수를 *h*(*x*)라고 할 때, 둘을 더한 f(x) = g(x) + h(x) 가 최소가 되는 지점을 우선적으로 탐색하는 방법이다. 이 f(x)가 작은 값부터 탐색하는 특성상 [우선순위 큐](https://namu.wiki/w/큐(자료구조)#s-3.2)가 사용된다. 휴리스틱 함수 h(x)에 따라 성능이 극명하게 갈리며, f(x) = g(x)일 때는 다익스트라 알고리즘과 동일하다.

   Q. 왜 쓰는가?

   A. 다익스트라는 실제 거리에 대한 비용을 이미 알고 시작한다. 현실에서는 그렇게 하기 어렵다. 그래서 휴리스틱 함수 h(x)를 쓰는 것이다. (기계학습에서도 많이 사용)

   

   ###### 다익스트라 구현.

   ![파일:LLFVSXa.gif](https://ww.namu.la/s/7cff087eb1f8876860f0d7a5e1747bd52eb9e20faff468bf3dbb9b267bd14a82602df9a6ef657a6bec140570b00efa1d8779c96fc3a6af1e9075f84ce3493c53413c7fbd60f8ba891e2c10c97009a62330f0c15fc84d71840777d44f0e53e57a)

출발지는 0, 나머지는 무한대로 세팅

![파일:J2C43pj.gif](https://w.namu.la/s/4e98f57a9b80f41aad785aa08b05c88f1380e88f3351d17c0145227fc4c69e39db4573bc6097fa7189ca455584a1ce96b9fa274bc3fbb672a8d960ceb070b791810039143a51c20fea51576be2608f9ea095c25eee3ac17b7ac0a73f0bd0eacc)

가장 가까운 B부터 방문 (Greedy), 방문하면서 relaxtion에 의해 값이 업데이트 됨

![파일:yaWRlZM.gif](https://ww.namu.la/s/a915731233ba006e765c8bce2fd56cdb0dda05fe2c3cab1020b4f0a3031d58d208973d4034e6e1d8e0bf73a8aeabec275b163417c9d7cdac22080413e1e126a21fddf40463a4086373448830472763f4132df2c0b6c5a9dcda402de20afdd225)

![파일:PfbUgIx.gif](https://w.namu.la/s/12e2bca491edeed1c5d1e6c9b5c13fd91973b580d68f8ff3a0997395d82f025ae46b7e5a1f66d67bc63127f9a742ddbe748e9c6cdd27faaa16bde9f88ab98552f025c9e657c64ec599236d491001ca0d7841752e924208c75c40a6adc9e82e45)

![파일:UGvHXBg.gif](https://w.namu.la/s/d6fbe1219d765106e87b61d0bf3ffbe1d0398ed40aee660dc430e30b854e8d62cdfbe5a47c40d8589dd959b2c327fbe58cfb56492b9d6a1249e79b89f346df45fb1a3cf195425e595fca69166da31ccbe9c691d71711500895b3680665ce623c)

#### 특성

- 네트워크에서 최단경로를 찾을 수 있다.

- 일반적으로 가장 빠른 알고리즘

- 균일 그래프(가중치가 없는 그래프)에서는 BFS를 사용하는게 더 빠를 수 있다.

- 음수의 가중치가 있을때는 적용하지 못한다.

  #### 음수의 가중치가 있으면?

  1. 무한 싸이클에 빠짐
  2. 탐색할 수 없는 경로 존재



### 플로이드 알고리즘

- 가중치의 부호에 관계없이 음의 사이클(negative cycle)만 존재하지 않으면 항상 사용할 수 있다

- All pairs

- 모든 정점에 대한 경로를 계산하므로 2차원 배열에 저장 (실제 경로, 최단 경로 따로 저장)

  #### 로직

  **1.** **2차원 배열을 만들고 그래프의 간선의 정보를 저장한다. (\* 두 정점이 직접적으로 연결되어 있지 않으면 INF(무한대)값, 자기 자신으로 가는 거리는 0으로 한다.)**

  **2. 경유지 1~V 까지 순회하여 2차원 테이블을 업데이트 한다.**

  1~2반복

  ```
  void Floyd_Warshall() {
    for(m=1; m<=N; m++)
      for(s=1; s<=N; s++)
        for(e=1; e<=N; e++)
           d[s][e] = d[s][e] > d[s][m] + d[m][e] ? d[s][m]+d[m][e] : d[s][e];
  }
  ```

  



### Refference

https://new93helloworld.tistory.com/217

[https://ratsgo.github.io/data%20structure&algorithm/2017/11/27/bellmanford/](https://ratsgo.github.io/data structure&algorithm/2017/11/27/bellmanford/)

[https://namu.wiki/w/A*%20%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98

https://yabmoons.tistory.com/365 [얍문's Coding World..]](https://namu.wiki/w/A* 알고리즘)

