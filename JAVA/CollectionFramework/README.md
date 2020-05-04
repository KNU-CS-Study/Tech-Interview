# 컬렉션 프레임워크

## 컬렉션 프레임 워크란?

자바에서 컬렉션 프레임워크란 **다수의 데이터를 쉽고 효과적으로 처리할 수 있는 표준화된 방법을 제공하는 클래스의 집합**을 의미합니다.

컬렉션은 다수의 데이터, 즉 데이터 그룹을, 프레임워크는 표준화된 프로그래밍 방식을 의미합니다.

즉, 데이터를 저장하는 자료 구조와 데이터를 처리하는 알고리즘을 구조화 하여 클래스로 구현해 놓은 것입니다.

이러한 컬렉션 프레임워크는 `자바의 인터페이스(interface)를 사용하여 구현`됩니다.



#### 주요 인터페이스 간의 상속 관계

![주요인터페이스상속관계](http://tcpschool.com/lectures/img_java_collection_interface_diagram.png)

이중에서 List와 Set 인터페이스는 모두 Collection 인터페이스를 상속받지만, 구조상의 차이로 인해 Map 인터페이스에 별도로 정의된다.



## 컬렉션 종류

<img src="https://user-images.githubusercontent.com/36303777/79859027-4f68db00-840b-11ea-9886-f66c8530630b.png" alt="image" style="zoom:33%;" />

| **인터페이스** | **설명**                                                     | **구현 클래스**                                |
| -------------- | ------------------------------------------------------------ | ---------------------------------------------- |
| List<E>        | 순서가 있는 데이터의 집합으로, 데이터의 중복을 허용한다.  예) 대기자 명단 | Vector, ArrayList, LinkedList, Stack, Queue 등 |
| Set<E>         | 순서가 없는 데이터의 집합으로, 데이터의 중복을 허용하지 않는다. 예) 양의 정수집합, 소수의 집합 | HashSet, TreeSet 등                            |
| Map<K, V>      | 키(Key)와 값(Value)의 한 쌍으로 이루어진 데이터의 집합으로 순서가 없다. 키는 중복을 허용하지 않지만 값은 중복될 수 있다. 예) 우편번호, 지역번호(전화번호) | HashMap, TreeMap, Hashtable, Properties        |



## List 컬렉션

* 객체를 일렬로 늘어놓은 구조
* 객체 저장시 자동 인덱스 부여
* 인덱스로 검색,삭제 할수있는 기능 제공.
* 객체자체를 저장하는 것이아니라 객체의 번지를 참조한다.
  * 즉, 인덱스마다 객체의 번지 주소가 들어있다. 동일한 객체를 중복 저장할 수있는데, 이 경우 동일한 번지가 참조되고 null이 저장될 경우에는 해당 인덱스는 객체를 참조하지 않는다.

### ArrayList

* 사용빈도가 아주 높은 컬렉션 클래스

* LIst인터페이스를구현하기 때문에 **데이터의 저장순서가 유지되고 중복을 허용한다.**

* Object 배열을 이용해서 데이터를 순차적으로 저장한다.

* 배열에 순차적으로 저장되며, 더이상 저장할 공간이 없으면 보다 **큰 새로운 배열을 생성해서 기존의 배열에 저장된 내용을 새로운 배열로 복사한 다음에 저장**한다.

* ~~~java
  List<String> list = new ArrayList<String>();//기본 생성자-> 초기 10개짜리 자동 생성
  List<String> list = new ArrayList<String>(30); //30개
  ~~~

* List 인터페이스는 제네릭 타입이다.

### LinkedList<E> 클래스

* 연결리스트를 이용하여 요소를 저장.
* 저장된 요소가 비순차적으로 분포. 이러한 요소들 사이를 링크로 연결하여 구성

### Vector <E> 클래스

* 기존코드와 호환성을 위해서 그냥 남아있다. 쓸필요없고 ArrayList와 같은동작을 수행하여 ArrayList를 쓰면된다.

### Stack<E> 클래스

* Vector 클래스를 상속받는다.
* 스택, LIFO

### Queue<E> 인터페이스

* 클래스로 구현된 스택과는 달리 별도의 인터페이스 형태로 제공된다. 

* Queue 인터페이스를 상속받는 하위 인터페이스

  1. Deque<E>

  2. BlockingDeque<E>
  3. BlockingQueue<E>

  4. TransferQueue<E>

* Deque인터페이스를 구현한 LinkedList클래스가 큐 메모리 구조를 구현하는 데 가장 많이 사용된다.



### ArrayList와 LinkedList의 차이

배열과 연결리스트 차이랑 같은거다. 삭제시 ArrayList는 한칸씩 다 당겨진다.

빈번한 객체의 삽입삭제시에는 LinkedList가 적합하다.



## Set 컬렉션

* 저장순서가 유지되지 않는다.
* 객체를 중복해서 저장할 수 없다. 
* 하나의 null만 저장할 수 있다.
* 대표적인 Set 인터페이스의 구현클래스 : HashSet, LinkedHashSet, TreeSet

### HashSet

* 객체를 **순서없이 저장**한다.
* 동일한 객체는 **중복 저장하지 않는다.**
  * HashSet은 객체를 저장하기 전에 먼저 객체의 hashCode() 메소드를 호출하여 해시코드를 얻어낸다. 그리고 이미 저장되어 있는 객체들의 해시코드와 비교한다. 만약 동일한 해시코드가 있다면 다시 equals() 메소드로 두 객체를 비교해서 true가 나오면 동일한 객체로 판단하고 중복 저장을 하지 않는다

### TreeSet 클래스

* 이진 검색 트리(binary search tree)의 형태로 요소를 저장
* 데이터가 정렬된 상태로 저장
* 데이터를 추가하거나 제거하는 등의 기본 동작 시간이 매우 빠르다
* JDK 1.2부터 제공되는 TreeSet 클래스는 NavigableSet 인터페이스를 기존의 이진 검색 트리의 성능을 향상시킨 레드-블랙 트리(Red-Black tree)로 구현
* TreeSet 클래스는 Set 인터페이스를 구현하므로, 요소를 순서에 상관없이 저장하고 중복된 값은 저장하지 않는다

### LinkedHashSet

* 중복된 데이터를 저장할 수 없다. 
* 입력된 순서대로 데이터를 관리한다.

## Map 컬렉션

* Key, value, pair 로 구성된 Entry를 객체를 저장하는 구조
* key와 value는 모두 객체
* key는 중복저장 불가능
* value는 중복 가능
* 기존키와 동일한 키로 값을 저장하면 기존값은 없어지고 새로운 값으로 대치된다.
* Map 컬렉션에는 HashMap, Hashtable, LinkedHashMap, Properties, TreeMap

### HashMap

* HashMap의 키로 사용할 객체는 hashCode()와 equals() 메소드를 재정의해서 동등 객체가 될 조건을 정해야 한다.
* 동등 객체, 즉 동일한 키가 될 조건은 hashCode()의 리턴값이 같아야 하고, equals() 메소드가 true를 리턴해야 한다.
* 주로 키타입은 String을 많이 사용하는데, String은 문자열이 같을 경우 동등 객체가 될 수 있도록 hashCode()와 equals() 메소드가 재정의되어 있다
* HashMap을 생성하기 위해서는 키 타입과 값 타입을 파라미터로 주고 기본 생성자를 호출하면 된다.

### HashTable

* HashMap과 동일한 내부 구조
* 키로 사용할 객체는 hashCode()와 equals() 메소드를 재정의해서 동등 객체가 될 조건을 정해야 합니다.
* **HashMap과의 차이점**은 Hashtable은 동기화된(Synchronized) 메소드로 구성되어 있기 때문에 멀티 스레드가 동시에 이 메소드들을 실행할 수는 없고, 하나의 스레드가 실행을 완료해야만 다른 스레드를 실행할 수 있습니다.

### Properties

* Hashtable의 하위 클래스이기 때문에 Hashtable의 모든 특징을 그대로 가지고 있습니다.
* 차이점은 Hashtable은 키와 값을 다양한 타입으로 지정이 가능한데 비해 Properties는 키와 값을 String 타입으로 제한한 컬렉션입니다.

### Reference

* https://steady-snail.tistory.com/74
* https://devbox.tistory.com/entry/Java-컬렉션-프레임워크
* https://deftkang.tistory.com/49
* https://lalwr.blogspot.com/2016/02/collection-framework.html
* https://palpit.tistory.com/656
* http://tcpschool.com/java/java_collectionFramework_concept