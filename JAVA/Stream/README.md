# Stream

> 데이터 처리 연산을 지원하도록 소스에서 추출된 연속된 요소



## JAVA8에서의 변경 사항

1. 람다표현식(lambda expression) : 함수형 프로그래밍
2. 스트림 API(Stream API) : 데이터의 추상화
3. Java.time 패키지 : Joda-Time을 이용한 새로운 날짜와 시간 API
4. 나즈혼(Nashorn) : 자바스크립트의 새로운 엔진.



이중 스트림 API 에 대해 자세히 다루어 보겠습니다.







## Stream API

### Stream API 이전

* 자바에서 많은 양의 데이터를 저장하기 위해서는 **배열이나 컬렉션을 사용.**
* 이러한 데이터를 접근하기 위해서는 **반복문이나 반복자(iterator)를 사용하여 매번 코드를 작성.**
* 이러한 코드들은 길고 가독성이 떨어지고 코드의 재사용이 불가능.



### Stream API

* 데이터를 추상화 하여 다룬다. 다양한 방식으로 저장된 데이터를 읽고 쓰기 위한 공통된 방법을 제공한다.
* 배열이나 컬렉션 뿐만 아니라 파일에 저장된 데이터도 모두 같은 방법으로 다룰 수 있다.



### Stream

* Array, Collections 와 같이 연속된 형태의 객체이다.
* 자료구조는 아이다.
* 입력받은 원래의 자료구조는 바꾸지 못한다.
  * 대신, 파이프라인 형태로 연결된 메소드의 결과를 제공한다.
* 최종 연산자(terminal operatoin)는 stream의 끝을 의미하며 모든 연산자를 수행한 결과를 반환한다.

~~~java
int result = list.stream()
  						.filter(...)
  						.map(...)
  						.count();
~~~

### 

## Create Operation

[자세한 operation 사용법](https://velog.io/@kskim/Java-Stream-API)



### Reference

* http://tcpschool.com/java/java_intro_java8
* https://velog.io/@kskim/Java-Stream-API