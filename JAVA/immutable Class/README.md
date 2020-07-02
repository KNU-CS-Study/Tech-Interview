# Immutable 클래스

> 변경이 불가능한 클래스이며, 가변적이지 않는 클래스.

## 특징

* 변경이 불가.
* 가변적이지 않다.
* 레퍼런스 타입의 객체이기 때문에 heap영역에 생성된다.
* 대표적으로 String, Boolean, Integer, Float, Long 등이 있습니다. 
* 재할당은 가능하다.
  * heap영역에서 변경불가능 한 것이지 재할당을 못하는 것은 아니다.
    * Ex) String a ="aa"; 에서 a ="bb";  로 재할당이 가능하다.
    * 위의 예제에서 a가 참조하고 있는 heap영역의 객체가 바뀌는 것이지 heap영역에 있는 값이 바뀌는 것이 아니다.
* **장점** : 생성자, 접근메소드에 대한 방어 복사가 필요없습니다. 멀티스레드 환경에서 동기화 처리없이 객체를 공유할 수 있습니다.  (Thread-safe)불변이기 때문에 객체가 안전합니다.
* **단점** : 객체가 가지는 값마다 새로운 객체가 필요합니다. 따라서 메모리 누수와 새로운 객체를 계속 생성해야하기 때문에 성능저하를 발생시킬 수 있습니다.



## 대표적인 Immutable : String

~~~java
String hi = "hi";
hi += "dongwook";
hi.concat("!!");
~~~

위의 코드들은 변경하는 것 처럼 보이지만 실제로는 새로운 String을 리턴한다. String은 속성중 value를 변경하지는 않는다. 이때 매번 객체를 새로 만든다.

만약 **변경이 잦은 경우**에는 

**StringBuffer나 StringBuilder 를 사용하는 것이 좋다.** 이 두 클래스는 mutable이다.

### StringBuffer, StringBuilder 차이 - 동기화 지원유무

String Buffer 는 멀티 쓰레드환경에서 synchronized키워드가 가능하므로 동기화가 가능하다. 즉, thread-safe하다.

반대로 StringBuilder는 thread-safe하지 않다.



## immutable 클래스를 만드는 방법

클래스의 필드가 final이거나 setter가 없으면 된다.

* final이면 뭐 setter가 있으나 없으나 상관없지만 여튼 그렇다.



### Reference 

* https://limkydev.tistory.com/68
* https://jeong-pro.tistory.com/85
