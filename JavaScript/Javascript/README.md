# JavaScript

>  자바스크립트(JavaScript)는 객체(object) 기반의 스크립트 언어입니다.

HTML로는 웹의 내용을 작성하고, CSS로는 웹을 디자인하며, 자바스크립트로는 웹의 동작을 구현할 수 있습니다.

자바스크립트는 주로 웹 브라우저에서 사용되나, Node.js와 같은 프레임워크를 사용하면 서버 측 프로그래밍에서도 사용할 수 있습니다.

현재 컴퓨터나 스마트폰 등에 포함된 대부분의 웹 브라우저에는 자바스크립트 인터프리터가 내장되어 있습니다.



## JavaScript의 특징

1. 자바스크립트는 **객체 기반의 스크립트 언어**입니다.

2. 자바스크립트는 **동적**이며, 타입을 명시할 필요가 없는 **인터프리터 언어**입니다.

3. 자바스크립트는 **객체 지향형 프로그래밍**과 **함수형 프로그래밍**을 모두 표현할 수 있습니다.



## JavaScript EventLoop

###  JavaScript Engine이란?

> JavaScript로 작성한 코드를 해석하고 실행하는 인터프리터

> 웹 브라우저에 화면을 그리는 **Rendering Engine**과 다르다.

자바스크립트 엔진은 기본적으로 하나의 쓰레드에서 동작한다. 하나의 쓰레드를 가지고 있다는 것은 하나의 stack을 가지고 있다는 의미와 같고, 하나의 stack이 있다는 의미는 `동시에 단 하나의 작업만을 할 수 있다`는 의미이다.

자바스크립트 엔진은 하나의 코드 조각을 하나씩 실행하는 일을 하고, 비동기적으로 이벤트를 처리하거나 Ajax 통신을 하는 작업은 사실상 Web API에서 모두 처리된다.

자바스크립트가 동시에 단 하나의 작업만을 한다는데 어떻게 여러가지 작업을 비동기로 작업을 할수 있을까?  `Event Loop와 Queue`

먼저 구글에서 개발한 V8을 비롯해 대부분의 자바스크립트 엔진은 크게 **세 영역**으로 나뉜다

* **Call Stack**
* **Task Queue(Event queue)**
* **Heap**

또한 추가적으로 `Event loop`가 task 들을 관리한다

![image](https://user-images.githubusercontent.com/42582516/80869487-a740f500-8cdb-11ea-9e6c-92110c7753e3.png)

#### Call stack

자바스크립트는 단 **하나의 호출 스택**을 사용한다. 이러한 특징 때문에 자바스크립트의 함수가 실행되는 방식을 "Run to Completion"라고 한다. 이는 **하나의 함수가 실행되면 이 함수의 실행이 끝날 때까지 다른 어떤 task도 수행될 수 없다**는 의미이다. 요청이 들어올 때마다 해당 요청을 순차적으로 호출 스택에 담아서 처리한다. 메소드가 실행될 때, Call Stack에 새로운 프레임이 생기고 **push**되고 메소드의 실행이 끝나면 해당 프레임은 **pop**되는 원리이다.

#### Heap

동적으로 생성된 객체(인스턴스)는 힙(heap)에 할당된다. 대부분 구조화되지 않는 '더미'같은 메모리 영역을 'heap'이라 표현

#### Task Queue(Event Queue)

자바스크립트의 런타임 환경에서는 처리해야하는 Task들을 임시 저장하는 대기큐가 존재한다. 그 대기 큐를 Task Queue 또는 Event Queue라고 한다. 그리고 Call Stack이 비어졌을 때 먼저 대기열에 들어온 순서대로 수행한다.

좀더 자세한 처리과정은 다음 주소에서 확인할 수 있다. [LINK](http://sculove.github.io/blog/2018/01/18/javascriptflow/)



## Hoisting

`hoist` 라는 단어의 사전적 정의는 끌어올리기 라는 뜻이다. 자바스크립트에서 끌어올려지는 것은 변수이다. `var` keyword 로 선언된 모든 변수 선언은 **호이스트** 된다. 호이스트란 변수의 정의가 그 범위에 따라 `선언`과 `할당`으로 분리되는 것을 의미한다. 즉, 변수가 함수 내에서 정의되었을 경우, 선언이 함수의 최상위로, 함수 바깥에서 정의되었을 경우, 전역 컨텍스트의 최상위로 변경이 된다.

> 추후 추가 예정

> https://developer.mozilla.org/ko/docs/Glossary/Hoisting



## Closure

Closure(클로저)는 **두 개의 함수로 만들어진 환경** 으로 이루어진 특별한 객체의 한 종류이다. 여기서 **환경** 이라 함은 클로저가 생성될 때 그 **범위** 에 있던 여러 지역 변수들이 포함된 `context`를 말한다. 이 클로저를 통해서 자바스크립트에는 없는 비공개(private) 속성/메소드, 공개 속성/메소드를 구현할 수 있는 방안을 마련할 수 있다.

> 추후 추가 예정

> https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Closures



## this에 대해

자바스크립트에서 모든 함수는 실행될 때마다 함수 내부에 `this`라는 객체가 추가된다. `arguments`라는 유사 배열 객체와 함께 함수 내부로 암묵적으로 전달되는 것이다. 그렇기 때문에 자바스크립트에서의 `this`는 함수가 호출된 상황에 따라 그 모습을 달리한다.

### 사용 상황 1. 객체의 메서드를 호출할 때



### 사용 상황 2. 함수를 호출할 때



### 사용 상황 3.  생성자 함수를 통해 객체를 생성할 때



### 사용 상황 4. apply, call, bind 를 통한 호출



## Promise

Javascript 에서는 대부분의 작업들이 비동기로 이루어진다. 콜백 함수로 처리하면 되는 문제였지만 요즘에는 프론트엔드의 규모가 커지면서 코드의 복잡도가 높아지는 상황이 발생하였다. 이러면서 콜백이 중첩되는 경우가 따라서 발생하였고, 이를 해결할 방안으로 등장한 것이 Promise 패턴이다. Promise 패턴을 사용하면 비동기 작업들을 순차적으로 진행하거나, 병렬로 진행하는 등의 컨트롤이 보다 수월해진다. 또한 예외처리에 대한 구조가 존재하기 때문에 오류 처리 등에 대해 보다 가시적으로 관리할 수 있다. 이 Promise 패턴은 ECMAScript6 스펙에 정식으로 포함되었다.

> 추후 추가 예정



## Async/Await

비동기 코드를 작성하는 새로운 방법이다. Javascript 개발자들이 훌륭한 비동기 처리 방안이 Promise로 만족하지 못하고 더 훌륭한 방법을 고안 해낸 것이다(사실 async/await는 promise기반). 절차적 언어에서 작성하는 코드와 같이 사용법도 간단하고 이해하기도 쉽다. function 키워드 앞에 async를 붙여주면 되고 function 내부의 promise를 반환하는 비동기 처리 함수 앞에 await를 붙여주기만 하면 된다. async/await의 가장 큰 장점은 Promise보다 비동기 코드의 겉모습을 더 깔끔하게 한다는 것이다. 이 것은 es8의 공식 스펙이며 node8LTS에서 지원된다(바벨이 async/await를 지원해서 곧바로 쓸수 있다고 한다!).

> 추후 추가 예정



## Arroy Function

화살표 함수 표현식은 기존의 function 표현방식보다 간결하게 함수를 표현할 수 있다. 화살표 함수는 항상 익명이며, 자신의 this, arguments, super 그리고 new.target을 바인딩하지 않는다. 그래서 생성자로는 사용할 수 없다.

> 추후 추가 예정



### References

* http://tcpschool.com/javascript/js_intro_basic
* https://github.com/JaeYeopHan/Interview_Question_for_Beginner/tree/master/JavaScript
* https://asfirstalways.tistory.com/362
* http://sculove.github.io/blog/2018/01/18/javascriptflow/

* https://developer.mozilla.org/ko/docs/Glossary/Hoisting

* https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Closures
