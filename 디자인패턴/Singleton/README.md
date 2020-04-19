# Singleton 패턴

## Singleton 패턴이란?

전역 변수를 사용하지 않고 **객체를 하나만 생성** 하도록 하며, 생성된 객체를 **어디에서든지 참조할 수 있도록** 하는 패턴. 즉, 생성자의 호출이 반복적으로 이뤄져도 실제로는 생성되는 객체는 최초 생성된 객체를 반환해 주는 것

`Singleton pattern(싱글턴 패턴)` 을 사용하지 않게되면 DBCP(DataBase Connection Pool )처럼 공통된 객체(쓰레드풀, 캐시, 대화상자, 사용자 설정, 레지스트리 설정, 로그 기록 객체 등)를 여러개 생성해서 사용해야하는 상황에서  인스턴스를 여러개 만들게 되면서 자원을 낭비하게 되거나 버그를 발생시킬 수 있다.

흔히 **자바**에서 많이 사용됨

#### 쓰는 이유

* 인스턴스가 절대적으로 한개만 존재하는 것을 보증하고 싶을 경우에 사용
* 두 번째 이용시부터 객체 로딩 시간이 현저하게 줄어 성능이 좋아짐

#### 문제점

* 너무 많은 일을 하거나 많은 데이터를 공휴시킬 경우, 다른 클래스의 인스턴스들 간에 결합도가 높아져 "개방-폐쇄 원칙"을 위배하게 된다.
  (객체 지향 설계 원칙에 어긋남 => 수정이 어려워지고 테스트하기 어려움)



## 구현

하나의 인스턴스만을 유지하기 위해 인스턴스 생성에 특별한 제약을 걸어둬야 한다. new를 실행할 수 없도록 생성자에 private 접근 제어자를 지정하고, 유일한 단일 객체를 반환할 수 있도록 정석 메소드를 지원해야 한다. 또한 유일한 단일 객체를 참조할 정적 참조변수가 필요하다. 

구현 방법은 아래의 **5개** 와 같다

### 1. Eager initialization (이른 초기화 방식)

Singletondml의 가장 기본적인 Eager initialization 방식이다. 먼저 클래스 내에 전역 변수로 instance 변수를 생성하고 private static을 사용하여 인스턴스화에 상관없이 접근이 가능하면서 동시에 private 접근 제어 키워드를 사용해 Eager initialization.instance로 바로 접근할 수 없도록 한다. 생성자에도 private 접근 제어 키워드를 붙여 다른 클래스에서 생성하는 것을 방지.

```java
package SingleTonExample;

public class EagerInitialization {
  private static EagerInitialization instance = new EagerInitialization();
  
  // 생성자
  private EagerInitialization() {}
  
  // 인스턴스 리턴
  private static EagerInitialization getInstance(){
    return instance;
  }
}
```

#### 장점

* static으로 생성된 변수에 싱글톤 객체를 선언했기 때문에 클래스 로더에 의해 클래스가 로딩될 때 싱글톤 객체가 생성
* 클래스 로더에 의해 클래스가 최초 로딩 될 때 객체가 생성됨으로 Thread-safe

#### 단점

* Singleton 객체 사용유뮤와 관계없이 클래스가 로딩되는 시점에서 항상 싱글톤 객체가 생성되고, 메모리를 잡고 있기 때문에 비효율적일 수 있음

### 2. Lazy initialization (늦은 초기화 방식)

Eager initialization (이른 초기화방식)과 정반대로 클래스가 로딩되는 시점이 아닌 클래스의 인스턴스가 사용되는 시점에서 Singleton 인스턴스를 생성함.

즉, 사용시점까지 Singleton 객체 생성을 미루기 때문에 사용하기 전까지 메모리를 점유하지 않는다. getInstance() 메서드안에서 instance가 null 인 경우에만 new LazyInitialization()을 선언함

```java
package SingleTonExample;

public class LazyInitialization {
  private static LazyInitialization instance;
  
  private LazyInitialization() {}
  
  private static LazyInitialization getInstance(){
    if(instance == null){
      instance = new LazyInitialization();
    }
    return instance;
  }
}
```

#### 장점

* Singleton 객체가 필요할 때 인스턴스를 얻을 수 있음.
* Eagle initialization 방식의 단점인 메모리 누수를 방지할 수 있음

#### 단점

* 만약 multi-thread 환경에서 여러 곳에서 동시에 getInstance()를 호출할 경우, 인스턴스가 두번 생성될 여지가 있음
* Multi-thread 환경에서는 Singleton 철학이 깨질 수 있는 위험



### 3. Thread safe Lazy initialization (스레드 안전한 늦은 초기화)

Lazy initialization 방식에서 thread-safe하지 않다는 단점을 보완하기 위해 멀티스레드에서 스레드들이 동시접근하는 동시성을 synchronized 키워드를 이용해 해결합니다.

```java
package SingleTonExample;

public class ThreadSafeLazyInitialization {
  private static ThreadSafeLazyInitialization instance;
  
  private ThreadSafeLazyInitialization() {}
  
  private static synchronized ThreadSafeLazyInitialization getInstance(){
    if(instance == null){
      instance = new ThreadsafeLazyInitialization();
    }
    return instance;
  }
}
```

#### 장점

* Lazy initialization 방식에서 thread-safe 하지 않은 점을 보완

#### 단점

* synchronized 키워드를 사용할 경우 자바 내부적으로 해당 역영이나 메서드를 lock, unlock 처리하기 때문에 내부적으로 많은 cost가 발생한다. 따라서 많은 thread 들이 getInstance()를 호출하게 되면 프로그램 전반적인 성능저하가 발생



### 3-1. Thread safe Lazy initialization + Double-checked locking 기법

위의 Thread safe Lazy initialization은 많은 스레드들이 동시에 synchronized 처리된 메서드로 접근하면 성능저하가 발생한다. 이를 좀 더 완화시키기 위해서 Double-checked locking기법을 사용한다.

첫번째 if문에서 instance가 null인 경우 synchronized 블럭에 접근하고 한번 더 if 문으로 instanc가 null 유무를 체크한다. 2번 모두다 instance가 null인 경우에 new를 통해 인스턴스화시킨다. instance가 null이 아니기 때문에 synchronized 블럭을 타지 않는다.

```java
package SingleTonExample;

public class ThreadSafeLazyInitialization {
  private static ThreadSafeLazyInitialization instance;
  
  private ThreadSafeLazyInitialization() {}
  
  private static ThreadSafeLazyInitialization getInstance(){
    if(instance == null){
      synchronized (ThreadsafeLazyInitialization.class){
        if(instance == null)
          instance = new ThreadsafeLazyInitialization();
      }
    }
    return instance;
  }
}
```

#### 장점

* Thread safe Lazy initialization 의 성능저하를 보완하였음

#### 단점

* 그래도 느린부분이 있음



### 4. Initialization on demand holder idiom (holder에 의한 초기화)

이 방법은 클래스안에 클래스(Holder)을 두어 JVM의 Class Loader 매커니즘과 Class가 로드되는 시점을 이용한 방법. Lazy initialization 방식을 가져가면서 Thread간 동기화 문제를 동시에 해결가능

중첩클래스 Holder는 getInstance 메서드가 호출되기 전에는 참조되지 않으며, 최초로 getInstance() 메서드가 호출될 때 클래스 로더에 의해 싱글톤 객체를 생성하여 리턴한다. holder안에 선언된 instance가 static이기 때문에 클래스 로딩 시점에 한번만 호출된다는 점을 이용. final을 사용했기 때문에 다시 값이 할당되지않음

```java
package SingleTonExample;

public class InitializationOnDemandHolderIdiom {
  private InitializationOnDemandHolderIdiom(){}
  
  private static class SingleTonHolder{
    private static final InitializationOnDemandHolderIdiom instance new InitializationOnDemandHolderIdiom();
  }
  
 public static InitializationOnDemandHolderIdiom getInstance() {
   return SingleTonHolder.instance;
 }
}
```

#### 장점

* 현재까지 **가장 많이 사용하는 방법**으로 알려짐, 그만큼 검증됬다.



### 5. Enum initialization (Enum 초기화)

자바 1.5버전부터 지원하는 Enum을 이용한 싱글톤 패턴을 구현

모든 enum type들은 프로그램 내에서 한번 초기화되는 점을 이용해 싱글톤을 구현함

```java
package SingleTonExample;

public enum EnumSingleTon {
  INSTANCE;
  public void excute (String arg){
    //...code
  }
}
```

#### 장점

* Eager initialization과 비슷한 장점
* Thread-safety와 Serialization이 보장됨
* Reflection을 통한 공격에도 안전함



## 정리

* Singleton 패턴은 Spring framework에서도 많이 사용되며, 어떤식으로 구현하는지 알아두면 도움이 된다
* 자바와 Spring에서의 Singleton 차이점은 Singleton 객체의 **생명주기**가 다르다.
* 자바에서 공유 범위는 Class loader 기준이지만, Spring에서는 ApplicationContext가 기준이 된다.



### References

* https://limkydev.tistory.com/67
* https://elfinlas.github.io/2019/09/23/java-singleton/
* https://gmlwjd9405.github.io/2018/07/06/singleton-pattern.html

