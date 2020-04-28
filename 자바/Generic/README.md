# Generic

### Generic이란?

제네릭은 다양한 타입의 객체들을 다루는 메서드나 컬렉션 클래스에 컴파일 시의 타입 체크를 해주는 기능이다.

즉, **클래스 내부에서 사용할 데이터 타입을 나중에 인스턴스를 생성할 때 확정하는 것**을 **제네릭**이라 한다.

객체의 타입을 컴파일 시에 체크하기 때문에 **객체의 타입 안정성**을 높이고 형변환의 번거로움이 줄어든다.

ArrayList와 같은 컬렉션 클래스는 다양한 종류의 객체를 담을 수 있긴 하지만 보통 한 종류의 객체를 담는 경우가 더 많다. 그런데도 꺼낼 때 마다 타입체크를 하고 형변환을 하는 것은 아무래도 불편할 수 밖에 없다.

![image](https://user-images.githubusercontent.com/42582516/80501989-100e3180-89ab-11ea-8575-341c1cd237ee.png)

> JDK1.5에 처음 도입되었다.



### Generic의 장점

1. 컴파일 시 강한 타입 체크를 할 수 있다.
   * 실행시 타입 에러가 나는 것보다 컴파일 시에 미리 타입을 강하게 체크해서 에러를 사전에 방지
2. 타입 변환(casting)을 제거한다.
   * 비제네릭 코드는 불필요하게 타입 변환을 하기 때문에 프로그램 성능에 악영향을 미친다.



### Generic 타입(class, interface)

제네릭 타입은 타입을 파라미터로 가지는 클래스와 인터페이스를 말한다.

클래스 또는 인터페이스 이름 뒤에 `<>` 부호가 붙고, 사이에 타입 파라미터가 위치한다.

> Object를 사용하는 비지네릭 타입은 모든 객체를 저장가능하다는 장점이 있지만, 저장할 때와 읽어 올때 타입 변환이 발생한다.

```java
public class 클래스이름<T> { ... }
public interface 인터페이스이름<T> { ... }
```

#### 멀티 타입 파라미터(class<K, V, ...>, interface<K, V, ...>)

제네릭 타입은 두 개 이상의 멀티 파라미터를 이용할 수 있다. 이 경우에는 각 타입 파라미터는 콤마로 구분한다.

```java
public class Entry implements Map.Entry<K,V>{
    private K key;
    private V value;  

    public Entry(K key, V value){
        this.key = key;
        this.value = value;
    }

    public K getKey(){ return this.key;}
    public V getValue(){ return this.value;}
    ....
}
```

#### 제네릭 메소드(<T, R> R method(T t))

제네릭 메소드는 **매개타입** 과 **리턴타입 **으로 **타입파라미터** 를 갖는 메소드를 말한다.

제네릭 메소드를 선언하는 방법은 리턴 타입 앞에 "<>" 기호를 추가하고 타입 파라미터를 기술한 다음, 리턴 타입과 매개 타입으로 타입 파라미터를 사용하면 된다.

```java
public <타입파라미터, ...> 리턴타입 메소드명(매개변수, ...) { ... }
public <T> Corn<T> makePopCorn(T t) { ... }

// 제네릭 메소드 호출 방법
Corn<Integer> = <Integer>makePopCorn(10); // 명시적으로 Integer를 지정
Corn<Integer> = makePopCorn(10); // Integer로 추정 (컴파일러가 매개 값을 보고 타입 추정)
```



#### 제한된 타입 파라미터(<T extends 최상위 타입>)

타입 파라미터에 지정되는 구체적인 타입은 제한될 필요가 있다.

예를 들어, 숫자를 연산하는 제네릭 메소드는 매개값으루 Number 타입 또는 하위 클래스 타입(Byte, Short, Integer, Long, Double)의 인스턴스만 가져야 한다. 이것이 제한된 타입 파라미터가 필요한 이유이다.

타입 파라미터 뒤에 extends 키워드를 붙이고 상위 타입을 명시한다. 상위 타입은 클래스 뿐만 아니라 **인터페이스**도 가능하다. (인터페이스라 implements를 사용하지 않는다.)

```java
public <T extends Number> int compare(T t1, T t2){
    double v1 = t1.doubleValue();
    ....
}
```



#### 와일드카드 타입(<?>, <? extends ...>, <? super ...>)

* 제네릭타입<?> : **제한 없음**
  * 모든 클래스나 인터페이스 타입이 올 수 있다.
* 제네릭타입<? extends 상위타입> : **상위 클래스 제한**
* 제네릭타입<? super 하위타입> : **하위 클래스 제한**



### References

* https://devbox.tistory.com/entry/Java-제네릭 [장인개발자를 꿈꾸는 :: 기록하는 공간]