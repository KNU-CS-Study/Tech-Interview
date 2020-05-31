# AOP

**AOP란 ?** 

> 애플리케이션에서 핵심적인 기능에서 부가적인 기능을 분리한다.

**Aspect Oriented Programming의 약자** 로, 관점 지향 프로그래밍이라고 불리기도 한다. 여러 객체에 공통으로 적용할 수 있는 기능을 분리해서 재사용성을 높여주는 프로그래밍 기법이다. AOP는 핵심 기능과 공통 기능의 구현을 분리함으로써 핵심 기능을 구현한 코드의 수정 없이 공통 기능을 적용 할 수 있게 만들어 준다. 

**관점 지향 프로그래밍이란 말을 바탕으로 다시 설명하자면 어떤 로직을 기준으로 핵심적인 관점, 부가적인 관점으로 난주어서 보고 그 관점을 기준으로 각각 모듈화하겠다는 것이다.**

>**모듈화란 ?** 어떤 공통된 로직이나 기능을 하나의 단위로 묶는 것을 말한다.

Aspect로 모듈화하고 핵심적인 비즈니스 로직에서 분리하여 재사용하겠다는 것이 AOP의 취지이다.

> 그럼 여기서 Aspect 는 무엇이냐? 
>
> AOP에서 부가적인 기능 을 Apect라고한다.
>
> 부가기능을 정의한 코드인 어드바이스(Advice)와 어드바이스를 어디에 적용할지 결정하는 포인트컷(PointCut)을 합친 개념이다.

쉽게 말하자면 중복된 코드를 최소화 시키고 이렇게 되면 유지보수까지 쉬워 진다고 보면된다. 



AOP의 기본개념은 핵심 기능에 공통 기능을 삽입 하는 것이다. 즉, 핵심 기능의 코드를 수정하지 않으면서 공통 기능의 구현을 추가하는 것이 AOP이다. **핵심 기능에 공통 기능을 삽입하는 방법**에는 다음 세가지가 있다.

## AOP 구현방법 3가지

* 컴파일 시점에 코드에 공통 기능을 삽입하는 방법
* 클래스 로딩 시점에 바이트 코드에 공통 기능을 삽입하는 방법.
* 런타임에 프록시 객체를 생성해서 공통 기능을 삽입하는 방법.(프록시패턴)



프록시 패턴 -> 스프링 AOP가 사용하는 방법.



## AOP 의 주요 개념 

* **Advice**
  * 타겟에 제공할 부가기능을 담고 있는 모듈
* **Join Point** 
  * Advice가 적용될 위치, 메서드 호출, 필드 값 변경 등이 Join Point에 해당한다.스프링은 프록시를 이용해서 AOP를 구현하기 때문에 메서드 호출에 대한 Join point만 지원한다.
  * 타겟 객체가 구현한 인터페이스의 모든 메서드는 조인 포인트가 된다.
* **Pointcut** 
  *  JoinPoint의 부분집합으로서 실제 Advice가 적용되는 Joinpoint를 나타낸다. 스프링에서는 정규 표현식이나 AspectJ의 문법을 이용하여 Pointcut을 정의할 수 있다.
* **Weaving** 
  * Advice 를 핵심 로직 코드에 적용하는 것을 weaving이라고 한다.
* **Aspect** 
  * 애스펙트는 AOP의 기본 모듈이다. 
  * 여러 객체에 공통으로 적용되는 기능을 Aspect라고 한다.
  * Aspect는 싱글톤 형태의 객체로 존재한다. 
  * 트랜잭션이나 보안 등이 Aspect의 좋은 예이다.



## Spring AOP 특징

1. Spring 은 프록시 기반 AOP를 지원한다.	
   * Spring은 타겟(target) 객체에 대한 프록시를 만들어 제공한다.
   * 타겟을 감싸는 프록시는 실행시간(Runtime)에 생성된다.
   * 프록시는 어드바이스를 타겟 객체에 적용하면서 생성되는 객체이다.
2. 프록시가 호출을 가로챈다.
3. Spring AOP는 메서드 조인 포인트만 지원한다.

## 프록시 패턴

실제 기능을 수행하는 객체 대신 가상의 객체(proxy object)를 사용해 로직의 흐름을 제어하는 디자인 패턴.



### 프록시 패턴의 특징

* 원래 하려던 기능을 수행하며 그외의 부가적인 작업(로깅, 인증, 네트워크 통신 등)을 수행하기에 좋다.
* 비용이 많이 드는 연산(DB 쿼리, 대용량 텍스트 파일 등)을 실제로 필요한 시점에 수행할 수 있다.
* 사용자 입장에서는 프록시 객체나 실제 객체나 사용법은 유사하므로 사용성이 좋다.



![image](https://user-images.githubusercontent.com/36303777/81706036-b6c5f800-94aa-11ea-9b83-d850d9acf6c4.png)

* Service 와 Proxy Object는 동일한 인터페이스를 구현합니다.
* Proxy 는 메서드 수행시 실제 객체(Service)의 메서드에 위임합니다.



![image](https://user-images.githubusercontent.com/36303777/81706755-29cf6e80-94ab-11ea-9e86-bafcbec55b8b.png)

위와 같이 구성된 도식을 직접 구현해 보면



~~~java
package org.springframework.samples.petclinic.proxy;

public interface Payment {
    void pay(int amount);
}

~~~



~~~ java
package org.springframework.samples.petclinic.proxy;

public class Cash implements Payment{

    public void pay(int amount){
        System.out.println(amount + " 현금 결제");
    }
}

~~~



~~~java
package org.springframework.samples.petclinic.proxy;

import org.springframework.util.StopWatch;

//프록시 클래스
public class CashPerf implements Payment{

    Payment cash = new Cash();
    @Override
    public void pay(int amount) {
        StopWatch stopWatch = new StopWatch();
        stopWatch.start();

        cash.pay(amount);

        stopWatch.stop();
        System.out.println(stopWatch.prettyPrint());



    }
}

~~~



~~~ java
package org.springframework.samples.petclinic.proxy;

public class Store {

    Payment payment;

    public Store(Payment payment) {
        this.payment = payment;
    }

    public void butSomething(int amount){
        payment.pay(amount);
    }
}

~~~



Test Class

~~~ java
package org.springframework.samples.petclinic.proxy;

import org.junit.jupiter.api.Test;

import static org.junit.jupiter.api.Assertions.*;

class StoreTest {


    //Cash 클래스와 Store클래스는 바뀌지 않았지만 이 코드 앞뒤로 성능 측정을 하도록 프록시 클래스를 이용함.
    @Test
    public void testPay(){
        Payment cashPerf = new CashPerf();
        Store store = new Store(cashPerf);
        store.butSomething(100);
    }
}

~~~



test class를 실행하면 



![image](https://user-images.githubusercontent.com/36303777/81707259-7b77f900-94ab-11ea-84c8-63b290582938.png)

위와 같이 나온다.



만약에 

~~~java 
Payment cashPerf = new CashPerf();
~~~

부분을 

~~~ java
Payment cashPerf = new Cash();
~~~

이렇게 다시 바꿔 프록시 객체를 빼버린다면



![image](https://user-images.githubusercontent.com/36303777/81707485-a7937a00-94ab-11ea-8f05-7b0834522872.png)

위와 같이 출력될 것이다. 



실제로 Cash클래스와 Store클래스는 바뀌지 않았지만 프록시클래스인 CashPerf를 이용하여 앞뒤로 성능 측정을 하도록 하였다.







### Reference

* 초보 웹 개발자를 위한 스프링 5 프로그래밍 입문 - 최범균 저
* https://engkimbs.tistory.com/746
* 인프런 예제로 배우는 스프링 입문 강좌
* https://refactoring.guru/design-patterns/proxy
* https://dong-co.tistory.com/84





