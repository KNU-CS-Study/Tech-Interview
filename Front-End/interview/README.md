# Front-End 면접 질문

## 일반적인 질문

- 어제/이번 주에 무엇을 공부하셨나요?
- 코딩을 할 때 당신을 들뜨게 하거나 흥미를 끄는 것들은 무엇은 가요?
- 최근에 당신이 경험한 기술적인 문제는 무엇이고 그것을 어떻게 해결했나요?
- 웹 애플리케이션이나 사이트를 만들 때 고려해야 할 UI, Security, Performance, SEO, Maintainability에 대해서 설명해주세요.
- 선호하는 개발 환경에 대해 자유롭게 이야기해 주세요.
- 버전 관리 시스템은 어떤 것들을 사용해보셨습니까?
- 당신이 웹 페이지를 만들 때의 과정을 설명해주실 수 있을까요?
- 당신에게 5가지 다른 stylesheet가 있습니다. 어떤 방법으로 사이트에 제공하는 게 가장 효과적일까요?
- 점진적 향상법(progressive enhancement)과 우아한 성능저하법(graceful degradation)의 차이를 설명하실 수 있습니까?
- 웹사이트에서 assets/resources를 최적화하는 방법에 관해 설명해주세요.
- 브라우저가 한 번에 1개의 도메인에서 내려받는 자원은 몇 개인가요?
  - 예외에는 어떤 것들이 있나요?
- 페이지 로드 시간을 줄이는 세 가지 방법에 관해서 이야기 해 보세요.
- 당신이 프로젝트에 합류했습니다. 근데 그들은 Tab을 이용하고, 당신은 Space를 사용했습니다. 어떻게 하실 건가요?
- 간단한 Slideshow 페이지를 만드는 방법에 관해서 이야기해 보세요.
- 만약 당신이 올해 기술적 책임자가 되었다면 무엇을 먼저 하시겠습니까?
- 표준의 중요성에 관해 설명해주세요.
- Flash of Unstyled Content에 관해 설명해주세요. 또 FOUC를 피하기 위해선 어떻게 해야 하나요?
- ARIA와 screenreader에 대해 설명해주세요. 또 접근성을 지원하는 웹사이트를 어떻게 만드는지에 대해도 설명해주세요.
- CSS 애니메이션과 JavaScript 애니메이션의 차이점에 관해 설명해주세요.
- CORS는 무엇의 약자이고 어떤 문제에 대해서 언급하는 것인가요?

## HTML 관련 질문

- `doctype`이 무엇을 하는 것인가요?
- 표준모드(standards mode)와 쿽스모드(quirks mode)의 다른 점은 무엇인가요?
- XML과 XHTML의 다른 점은 무엇인가요
- XHTML을 이용한 페이지의 한계점은 무엇이 있나요?
- `application/xhtml+xml`으로 지정한 페이지에 어떠한 문제가 있나요?
- 다국어가 포함된 페이지는 어떤 방식으로 제공하나요?
- 다국어 페이지를 제공하는 여러 방법에 관해 설명해주세요.
- `data-`속성은 무엇을 하는 것인가요? 사용했을 때 이점은 무엇인가요?
- HTML5를 오픈 웹 플랫폼(open web platform)으로 생각해본다면, 어떤 것들로 구성돼 있을까요?
- `쿠키(Cookies)`와 `세션저장소(sessionStorage)`와 `로컬저장소(localStorage)`의 차이점을 설명해주세요.
- `,`와 ``의 차이점에 관해 설명해주세요.
- CSS`를`사이에 쓰는 것과 JS`를`뒤에 사용하는 것은 좋은 사용법일까요? 어디에 배치하는 게 좋을까요?
- Progressive rendering이란 무엇인가요?
- 이미지 태그에 `srcset` 속성을 사용하는 이유는 무엇인가요? 브라우저가 이 속성을 가진 콘텐츠를 평가할 때 사용하는 과정을 설명해보세요.
- HTML templating language를 사용해 본 경험이 있나요?

## CSS 관련 질문

- class와 id의 차이점에 관해서 설명해주세요.
- “reset” CSS가 무엇인지, 어떻게 유용한지 설명해주세요.
- Floats가 어떻게 동작하는지 설명해주세요.
- z-index에 관해 설명해주세요.
- BFC(Block Formatting Context)에 관해 설명해주세요
- 클리어링(Clearing) 기술에는 어떤 것들이 있으며, 어떨 때 어떻게 사용하는 것이 적절한지 설명하세요.
- CSS 스프라이트(CSS Sprites)를 설명하고, 페이지나 사이트를 어떻게 향상하는지 설명하세요.
- Image Replacement를 사용해야 할 때, 선호하는 기술과 언제 사용하는지를 설명해주세요.
- 브라우저 스펙 차이에 따른 스타일링 이슈를 수정하기 위해서 어떻게 접근하나요?
- 기능이 제약된 브라우저를 위해서 어떤 방식으로 페이지를 만드나요?
  - 어떠한 기술과 절차를 거치는지 설명하세요.
- 시각적으로 보이지 않고 스크린 리더에서만 가능하게 하는 방법에 관해 설명해주세요.
- 그리드 시스템(Grid system)을 사용한 적이 있나요? 있다면 어떠한 것을 선호하나요?
- 미디어 쿼리(media queries)를 사용한 적이 있나요? 혹은 모바일에 맞는 layout과 CSS를 사용한 적이 있나요?
- SVG를 스타일링하는데 익숙하신가요?
- 인쇄하기 위해 웹페이지를 어떻게 최적화 하나요?
- 효율적인 CSS를 작성하기 위한 "비법(gotchas)"은 어떤 게 있나요?
- CSS 전처리(CSS preprocessors)를 사용해보셨나요?
  - 그렇다면, 사용 경험에 기반을 둬 좋았던 점과 나빴던 점을 설명해주세요.
- 페이지에서 표준 폰트가 아닌 폰트 디자인을 사용할 때 어떤 방식으로 처리하시나요? (웹폰트를 제외하고)
- CSS Selector가 어떠한 원리로 동작하는지 설명해주세요.
- pseudo-elements에 관해서 설명하고 어디에서 사용되는지 이야기해보세요.
- box model에 관해 설명하고 브라우저에서 어떻게 동작하는지 설명해주세요.
- `* { box-sizing: border-box; }`은 무엇이고 사용했을때 이점은 무엇인가요?
- 기억나는 display 속성에 대한 값들을 나열해보세요.
- inline과 inline-block의 차이점은 무엇인가요?
- 요소를 배치하는 방법(relative, fixed, absolute, static) 간의 차이는 무엇인가요?
- CSS에서 'C’는 Cascading을 의미합니다. Cascading에 관해서 설명해주세요. 또 cascading system의 장점은 무엇인가요?
- CSS framework를 사용해본 적이 있으신가요? 실무에서 사용해보았다면 어떤 이점이 있었나요?
- 새로운 CSS Flexbox 혹은 Grid 스펙을 사용해 보신 적 있나요?
- 반응형(Responsive) 디자인은 적응형(Adaptive) 디자인과 어떤 차이점이 있나요?
- 레티나 그래픽 환경에서 작업해 보신 적이 있나요? 하셨다면 어떤 기술을 사용하셨나요?
- *절대 좌표*대신 `translate()` 혹은 반대로 사용하는 이유가 있나요? 있다면 이유에 관해서 설명해주세요.

## JS 관련 질문:

- event delegation에 관해 설명해주세요.

- `this`는 JavaScript에서 어떻게 작동하는지 설명해주세요.

- prototype 기반 상속은 어떻게 하는지 설명해주세요.

- AMD와 CommonJS는 무엇이고, 이것들에 대해 어떻게 생각하시나요?

- 다음 코드가 즉시 호출 함수 표현식(IIFE)로 동작하지 않는 이유에 관해서 설명해보세요:

  ```
  function foo(){ }();
  ```

  - IIFE로 만들기 위해서는 어떻게 해야 하나요?

- `null` 과 `undefined` , `undeclared` 의 차이점은 무엇인가요?

  - 두개를 구분하기 위해서는 어떻게 하면 될까요?

- 클로져(Closure)는 무엇이며, 어떻게/왜 사용하는지 설명해주세요.

  - 클로져를 만들 때 선호하는 패턴은 무엇인가요? argyle (IIFEs에만 적용할 수 있다)

- 익명함수(anonymous functions)는 주로 어떤 상황에서 사용하나요?

- 당신의 코드를 어떻게 구성하는지? (모듈 패턴, 전통적 상속)

- 호스트 객체(Host Objects)와 네이티브 객체(Native Objects)의 차이점은 무엇인가요?

- 다음 코드의 차이점은 무엇인가요?

```javascript
function Person(){} var person = Person() var person = new Person()
```

- `.call`과 `.apply`의 차이점은 무엇인가요?
- `Function.prototype.bind`을 설명하세요.
- `document.write()`는 언제 사용하나요?
- UA 문자열을 이용하여 기능 검출(feature detection)과 기능 추론(feature inference)의 차이점을 설명하세요.
- AJAX에 관해 가능한 한 자세히 설명하세요.
- AJAX를 사용했을 때의 장단점에 대해 설명해주세요.
- JSON이 어떻게 동작 되는지 설명하세요. (그리고 AJAX와 어떻게 다른지 설명하세요.)
- 기존에 JavaScript 템플릿을 사용한 적이 있나요? 만약에 있다면, 어떠한 방식으로 사용했는지 말씀해주세요.
- "호이스팅(Hoisting)"에 대해서 설명하세요.
- 이벤트 버블링(Event Bubbling)에 대해서 설명하세요.
- 이벤트 캡쳐링(Event Capturing)에 대해서 설명하세요.
- "속성(Attribute)"와 "요소(property)"의 차이가 무엇인가요?
- 내장된 JavaScript 객체를 확장하는 것이 좋지 않은 이유는 무엇인가요?
- document load event와 DOMContentLoaded event의 차이점은 무엇인가요?
- `==`와 `===`의 차이점은 무엇인가요?
- JavaScript의 "동일출처정책(the same-origin policy)"에 대해서 설명하세요.
- 다음 코드를 동작하게 만드세요.

```javascript
duplicate([1, 2, 3, 4, 5]); // [1,2,3,4,5,1,2,3,4,5]
```

- 삼항식(Ternary statement)을 사용하는 이유는 무엇이고, 그것을 표현하기 위한 연산자 단어는 무엇인가요?
- `use strict;`은 무엇이고, 사용했을 때 장단점에 관해서 설명해주세요.
- 100번 반복되는 반복문이 있습니다. 3의 배수일 때는 `fizz`, 5의 배수일 때는 `buzz`, 3과 5의 공배수일 때는 `fizzbuzz`가 출력되는 코드를 작성해보세요.
- 전역 scope를 사용했을 때 장단점에 관해 설명해주세요.
- 때때로 `load` event를 사용하는 이유에 관해 설명해주세요. 또 단점이 있다면 대안에 대해서도 설명해주세요.
- SPA에서 SEO에 유리하도록 만들기 위한 방법에 대해 설명해주세요.
- Promise를 사용해 본 경험이 있나요?
- Promise가 콜백 대비 장/단점은 무엇인지 설명해주세요.
- JavaScript의 작동방식의 장단점에 관해 설명해주세요.
- JavaScript를 디버깅할 때 사용하는 도구가 있으면 설명해주세요.
- 객체 안의 속성과 배열의 아이템을 순회할 때 사용하는 문법에 관해 설명해주세요.
- mutable object와 immutable object에 관해 설명해주세요.
  - JavaScript에서 immutable 객체의 예를 들어보세요.
  - immutability의 장/단점은 무엇인가요?
  - 자신의 코드에서 불변성(immutability를) 어떻게 달성할 수 있나요?
- 동기방식과 비동기 방식 함수의 차이에 관해서 설명해주세요.
- event loop이란 무엇인가요?
  - call stack과 task queue에 관해 설명해주세요.
- `function foo() {}`와 `var foo = function() {}`에서 foo 의 차이가 무엇인지 설명해보세요.
- `let`, `var`, `const`의 차이점에 관해서 설명해주세요.

## 테스트 관련 질문들:

- test code를 작성하면서 개발하는 방식의 장점과 단점에 대해 설명해주세요.
- test code를 테스트하는 툴을 사용해보신 경험이 있나요?
- 유닛 테스트와 함수테스트의 차이점은 무엇인가요?
- code style linting tool을 사용했을때 장점은 무엇인가요?

## 성능 관련 질문들:

- 성능관련 이슈들을 발견하기 위해서 사용하는 방법은 무엇인가요?
- 웹사이트 scrolling 성능을 향상시키기 위한 몇가지 방법에 대해 설명해보세요.
- 브라우저의 layout, painting, compositing에 대해 설명해보세요.

## 네트워크 질문들:

- 전통적으로, 웹사이트의 assets을 여러 도메인으로 서빙했을 때 장점은 무엇인가요?
- URL로 접속했을 때 어떤 플로우로 화면에 웹사이트가 그려지는지 네트워크 관점에서 설명해주세요.
- Long-Polling과 Websocket, Server-Sent Event에 대해 설명해주세요.
- 다음 request header들에 대해 설명해주세요.
  - Diff. between Expires, Date, Age and If-Modified-…
  - Do Not Track
  - Cache-Control
  - Transfer-Encoding
  - ETag
  - X-Frame-Options
- HTTP와 HTTPS에 대해 설명해주세요.
- HTTP Method들에 대해 설명해주세요.

## 코딩 질문:

_질문: `foo`의 값은 무엇인가요?_

```javascript
var foo = 10 + "20";
```

_질문: 아래 코드의 결과값은 무엇인가요?_

```javascript
console.log(0.1 + 0.2 == 0.3);
```

_질문: 아래 코드가 동작하게 하기 위해선 어떻게 해야할까요?_

```javascript
add(2, 5); // 7
add(2)(5); // 7
```

_질문: 아래 구문의 반환값은 무엇인가요?_

```javascript
"i'm a lasagna hog".split("").reverse().join("");
```

_Question: What is the value of `window.foo`?_
_질문: `window.foo`의 값은 무엇인가요?_

```javascript
window.foo || (window.foo = "bar");
```

_질문: 아래 두 alert의 결과값은 무엇인가요?_

```javascript
var foo = "Hello";
(function () {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

_질문: `foo.length`의 값은 무엇인가요?_

```javascript
var foo = [];
foo.push(1);
foo.push(2);
```

_질문: `foo.x`의 값은 무엇인가요?_

```javascript
var foo = { n: 1 };
var bar = foo;
foo.x = foo = { n: 2 };
```

_질문: 아래 코드의 출력값은 무엇인가요?_

```javascript
console.log("one");
setTimeout(function () {
  console.log("two");
}, 0);
console.log("three");
```

## 그 외 흥미로운 질문들

- 최근에 수행했던 흥미로운 프로젝트는 무엇인가요?
- 사용하는 개발 도구에서 마음에 드는 부분은 무엇인가요?
- 프론트엔드 커뮤니티에서 당신에게 영감을 준 사람이 있다면 누구인가요?
- 애완동물 관련 프로젝트를 해 보았나요? 해보았다면 어떤 종류의 프로젝트인가요?
- IE에서 가장 좋아하는 기능은 무엇인가요?
- 어떤 커피를 좋아하시나요?

### References

- https://h5bp.org/Front-end-Developer-Interview-Questions/translations/korean/

---

## 일반적인 질문

- 어제/이번 주에 무엇을 공부하셨나요?

  생략

* 코딩을 할 때 당신을 들뜨게 하거나 흥미를 끄는 것들은 무엇은 가요?

  clean coding

- 최근에 당신이 경험한 기술적인 문제는 무엇이고 그것을 어떻게 해결했나요?

  생각해보기

* 웹 애플리케이션이나 사이트를 만들 때 고려해야 할 UI, Security, Performance, SEO, Maintainability에 대해서 설명해주세요.

  **UI** : PC와 모바일 사이트를 하나의 도메인에서 서비스를 하려면 반응형 디자인으로 페이지를 구현해야 합니다. 그렇지 않으면 두개의 도메인을 구분하여 PC용과 Mobile 용을 따로 디자인하여 퍼블리싱하여야한다.

  **Security** : 웹 사이트 보안은 다양한 종류의 공격을 방지하는 것. 웹 사이트를 설계하는 과정에서 다양한 보안적인 측면을 고려해야 한다. 그러나 일반적으로 서버측 웹 프레임워크를 사용하면 일반적인 보안 공격에 대해 검증된 방어 메커니즘이 기본적으로 제공한다. 다른 공격들은 HTTPS를 활성화하는 등의 웹 서버 설정을 통해 방지할 수 있다. 마지막으로 공개된 취약점 스캐너 도구를 사용하여서 알려진 보안 실수를 해결할 수 있을 것이다.

  다양한 위협 : XSS, SQL injection, CRSF, DoS 등

  **Performace** : FE에서 성능향상을 위해서는 기본적으로 첫번 째는 우선 style 태그는 태그 내에, script 태그는 최하단에 배치시키는 것. 이렇게 해야지 브라우저에 의해 DOM이 생성되고 렌더링 되면서 우선적으로는 style이 적용되어야 하고, script는 마지막에 불러와 로직이 적용되어야하기 대문이다.

  두번째는 FE프레임워크마다 다르지만 Vitual DOM을 사용하는 것이다. Angular의 경우는 Virtual DOM을 기본스펙으로 하지 않기 때문에 페이지를 리플로우 / 리드로우 할 때 체감상 상당히 느리게 느껴진다. 그러나 Vue.js 나 React.js 의 경우는 Virtual DOM을 사용하기 때문에 리플로우 / 리드로우를 하는 경우 시간을 최소화 할 수 있다.

  마지막으로 프로젝트를 완료 후 빌드할 때에는 공통적으로 Uglify, Minify, Gzip 프로세스를 추가하여 브라우저에서 JS나 CSS를 로드할 때의 시간을 최소화하며 성능향상을 기대할 수 있다.

  이외에도 다양한 방법들이 있다. 성능 최적화, 중요 렌더링 경로 분석 및 최적화, 렌더링 차단 CSS 피하기, 자바 스크립트 최적화, 내이게이션 타이밍으로 측정, 다운로드 횟수를 줄이기, 텍스트 크기 줄이기, 이미지 최적화, HTTP 캐싱 등등

  > 관련 출처 : https://writingdeveloper.tistory.com/247

  **SEO** : 검색엔진최적화(Search Engine Optimization, SEO)

  검색엔진을 최적화 하기 위해 `<title>` 태그와 `<meta>` 태그에 대한 정보를 모두 입력한다. 또한 `robots.txt` 을 사용한다. `<a>` 태그를 사용한다.

  > robots.txt 는 검색로봇에게 사이트 및 웹페이지를 수집할 수 있도록 허용하거나 제한하는 국제 권고안

  **Maintainability** : 코드 컨벤션을 정의한다. 이는 팀원들간의 유지보수를 쉽고 빠르게 유지할 수 있습니다. 간단하게는 네이밍부터 HTML, CSS, Javascript 까지 정의한다. `linter` 을 사용해서 할 수 있다. 여러 종류의 linter가 있지만 린터를 사용하였을 때 유지보수가 용이하고 코드의 질이 올라간다.

- 선호하는 개발 환경에 대해 자유롭게 이야기해 주세요.

  일반적으로 웹개발을 진행할 때, Mac을 선호한다. 최근에 Mac을 사용하게 되었는데 Homebrew가 너무 편하다. 주로 사용하는 IDE 는 `Visual Studio Code` 이다.

  > Homebrew는 apple이나 리눅스에서 제공하지 않는 유용한 패키지 관리자를 설치

* 버전 관리 시스템은 어떤 것들을 사용해보셨습니까?

  일반적으로 git을 사용합니다. git을 통해 다양한 협업을 진행한 경험이 있으며 git flow나 github flow에 관심이 있습니다. 현재도 1일 1커밋을 진행하면서 git이 익숙합니다.

- 당신이 웹 페이지를 만들 때의 과정을 설명해주실 수 있을까요?

  실제적인 협업을 작업해 본적은 없습니다. 대략적인 단계는 다음과 같이 진행합니다. 기획과 디자인을 먼저 한 후 퍼블리싱을 진행합니다. 퍼블리싱을 작업하여 반응형일 경우 모바일과 PC버전의 화면을 체크하고 MockData를 삽입하여 실제 데이터가 표시된 것처럼 작업합니다. 이후 로직단을 작업하며 RESTFul API를 통해 데이터를 가져오거나 추가 로직을 입힙니다. 이후 UI와 로직 모두 테스팅을 진행하며 시나리오 대로 페이지가 동작하는지 확인합니다.

  > 웹 퍼블리싱(Web Publishing)이란? 웹 퍼블리싱이란 디자이너로부터 전달받은 시안을 웹브라우저에서 볼 수 있도록 웹문서화 하는 코딩 작업
  >
  > http://websrepublic.co.kr/news/4

* 당신에게 5가지 다른 stylesheet가 있습니다. 어떤 방법으로 사이트에 제공하는 게 가장 효과적일까요?

  CSS는 런타임시 조작 가능한 선언형 언어입니다. 그러므로 각 스타일시트를 컴파일할 수 있는 프리컴파일러를 만들거나 SASS나 SCSS 등을 통하여 하나의 스타일시트로 병합한 후 제공합니다.

- 점진적 향상법(progressive enhancement)과 우아한 성능저하법(graceful degradation)의 차이를 설명하실 수 있습니까?

  **점진적 향상법(progressive enhancement)** 은 많은 테스팅을 통해 기능을 점진적으로 향상시키는 것을 의미합니다.

  **우아한 성능저하법(graceful degradation)** 은 최신기기에서 동작하는 기능을 만들고 난 다음에 오래된 기기에서 동작할 수 있도록 다른 버전을 두어 관리 또는 만드는 것을 의미합니다.

* 웹사이트에서 assets/resources를 최적화하는 방법에 관해 설명해주세요.

  - CDN을 사용

    > CDN : 콘텐츠 전송 네트워크, 콘텐츠를 효율적으로 전달하기 위해 여러 노드를 가진 네트워크에 데이트를 저장하여 제공하는 시스템

  - Cache Expiration(캐쉬 만료) 명시

    > Cache Expiration : 캐쉬에 저장된 데이터가 오래된 경우 서버로 재요청, 캐쉬 만료전까지는 서버에 요청할 필요가 없으므로 네트워크 요청에 대한 왕복(roundtrip)시간을 절약할 수 있다.)

  - Sprite 이미지 생성을 통한 HTTP Request 최소화

    > Image sprite란 여러 개의 이미지를 하나의 이미지로 합쳐서 관리하는 이미지를 의미. 사용된 이미지가 많을 경우 웹 브라우저는 서버에 해당 이미지의 수만큼 요청해야만 하므로 휍 페이지의 로딩 시간이 오래 걸리게 된다.
    >
    > http://tcpschool.com/css/css_basic_imageSprites

  - 빌드, 번들링 도구를 이용하여 자바스크립트, CSS 등을 compress하여 제공

    > ex) Javascript의 webpack. webpack은 모듈 시스템을 구성하는 기능 외에도 로더 사용, 빠른 컴파일 속도 등 장점이 많습니다.
    >
    > JavaScript에 모듈화 시스템을 적용하려는 많은 노력이 있습니다. JavaScript 모듈화 명세를 만드는 대표적인 작업 그룹에 [CommonJS](http://www.commonjs.org/)와 [AMD(Asynchronous Module Definition)](https://github.com/amdjs/amdjs-api/wiki/AMD)가 있습니다. [webpack](http://webpack.github.io/)은 두 그룹의 명세를 모두 지원하는 JavaScript 모듈화 도구입니다.
    >
    > ![그림 1 컴파일 과정](https://d2.naver.com/content/images/2016/02/webpack-1.png)
    >
    > [webpack의 컴파일 과정]

  - script는 body 가장 아래에 스타일은 header에 명시하고 또한 캐시 적용 가능한 외부 링크를 통해서 제공

  - 타입에 맞는 이미지 포맷 사용 및 메타 데이터를 제거

  - 리다이렉트를 피하기

    > 사용자를 한 URL에서 다른 URL로 다시 보내는 것을 의미. 이는 페이지를 더 느리게 만듦
    >
    > 피하는 다양한 방법 : 주소 뒤 슬래시 빼기, Alias 등의 웹사이트 연결, 내부 트래픽 추적, 외부 트래픽 분석, 간단한 URL 등등

- 브라우저가 한 번에 1개의 도메인에서 내려받는 자원은 몇 개인가요?

  브라우저마다 다르다. 일반적으로 평균 6~8개의 리소스를 동시에 받을 수 있다. 크로스 브라우징을 고려하면 평균적으로 6개라고 생각하면 된다.

  1개의 도메인에서 다운받는 리소스는 HTML문서, CSS, Javascript, Web font, Media 등 8가지 정도가 있는 것으로 알고 있습니다.
  HTTP1.0의 경우 TCP 커넥션을 4개까지 지원하지만 커넥션의 생성, 소멸에 따른 비용 때문에 HTTP1.1의 경우 TCP 커넥션을 2개 지원하고 있습니다. 커넥션의 수에 따라 데이터를 받아오는 폭도 달라지겠지만 DNS Lookup에 따른 비용도 발생하기 때문에 많은 도메인에서 데이터를 제공하는것은 오히려 성능 저하가 발생할 수 있으므로 2개 정도의 도메인에서 제공하는 것이 효율적으로 알고 있습니다.

  > 크로스 브라우징 : 적어도 표준 웹기술을 채용하여 다른 기종 혹은 플랫폼에 따라 달리 구현되는 기술을 비슷하게 만듦과 동시에 어느 한쪽에 최적화되어 치우지지 않도록 공통 요소를 사용하여 웹 페이지를 제작하는 기법을 말하는 것

  - 예외에는 어떤 것들이 있나요?

    > https://programmingsummaries.tistory.com/285

* 페이지 로드 시간을 줄이는 세 가지 방법에 관해서 이야기 해 보세요.

  1. HTTP 요청 줄이기
  2. CSS 스프라이트(sprite)
  3. CDN의 사용
  4. 캐시 만료일 설정
  5. Gzip 사용
  6. 상단에 스타일시트 넣기
  7. 하단에 스크립트 넣기
  8. JavaScript 와 CSS 파일을 외부로 분리하기
  9. Javascript 와 CSS 통합하기
  10. JavaScript and CSS Minify(축소)
  11. DNS 조회 줄이기
  12. 중복 Script 줄이기
  13. 리다이렉트 피하기
  14. ETag 헤더를 설정
  15. 초기 렌더링 시 Ajax 요청 최소화하기
  16. 쿠키 사이즈 줄이기
  17. 구성요소들에 대해 cookie-free 도메인을 사용하기
  18. iframe의 개수를 최소화 하기
  19. DOM 요소의 수를 줄이기
  20. DOM 접근을 최소화 하기
  21. 이벤트 핸들러 설정
  22. NO 404s 없애기
  23. CSS filter, CSS Expression 사용 자제
  24. HTML에서 이미지 크기를 줄이지 않기 등등

  출처 : https://bearjin90.tistory.com/21

  다른 자료 1 : [https://seosem.kr/검색엔진최적화-웹페이지-로딩속도를-개선-5가지](https://seosem.kr/%EA%B2%80%EC%83%89%EC%97%94%EC%A7%84%EC%B5%9C%EC%A0%81%ED%99%94-%EC%9B%B9%ED%8E%98%EC%9D%B4%EC%A7%80-%EB%A1%9C%EB%94%A9%EC%86%8D%EB%8F%84%EB%A5%BC-%EA%B0%9C%EC%84%A0-5%EA%B0%80%EC%A7%80/)

  다른 자료 2 : https://www.webhostingsecretrevealed.net/ko/blog/inbound-marketing/8-tips-to-speed-up-your-website/

- 당신이 프로젝트에 합류했습니다. 근데 그들은 Tab을 이용하고, 당신은 Space를 사용했습니다. 어떻게 하실 건가요?

  팀의 코드 컨벤션을 유지합니다. 제가 우선시하는 것은 개인적인 성향보다는 팀원들간의 커뮤니케이션이고 다른 사람의 코드를 볼때 빠른 이해가 중요합니다. 이를 위해 Tab이 서로간에 코드를 이해하는 것이 빠르다면 Tab을 사용할 것입니다. 또한 이러한 경우 대부분 ESLint를 주로 사용하여 코드 컨벤션을 유지합니다.

* 간단한 Slideshow 페이지를 만드는 방법에 관해서 이야기해 보세요.

  position: absolute; left: width; 를 기반으로 모든 페이지를 좌측으로 정렬 시키고, 자바스크립트로 left 값을 변경하는 식.
  직접 스타일을 조작하는데 리플로우, 리드로우와 같이 퍼포먼스 문제가 있다면 CSS3 transform을 사용합니다.

- 만약 당신이 올해 기술적 책임자가 되었다면 무엇을 먼저 하시겠습니까?

  페어 프로그래밍? 새로운 기술의 도입?

* 표준의 중요성에 관해 설명해주세요.

  표준을 정의함으로서 팀원들 간에는 서로의 코드를 이해하고 수정하는 시간을 줄일 수 있다. 또한 코드를 작성한 개발자가 사정이 생기더라도 표준에의한 코딩을 함으로서 쉽게 다른 개발자가 코딩을 할 수 있게한다.

- Flash of Unstyled Content에 관해 설명해주세요. 또 FOUC를 피하기 위해선 어떻게 해야 하나요?

  FOUC(Flash of Unstyled Content)는 브라우저로 웹문서에 접근했을때, 미처 CSS의 스타일이 모두 적용되지 못한 상태에서 화면이 표시되어 발생하는 화면 깜박임, 스타일의 적용 전과 적용 후가 그대로 화면에 노출된 상태로 변경되는 현상등을 일컫는다. 이 현상은 특히 IE(Internet Explorer) 브라우저에서 확인되는데 최신의 IE11에서도 여전히 발생되는 문제이다. 이는 해당 웹문서의 사용자 경험을 떨어뜨리는 요인으로 작용한다.

  **FOUC 해결책**은 다음과 같다.

  - FOUC를 최소화하기 위해서는 기본적으로 `<head>` 요소안에 CSS를 링크하고, @import의 사용을 자제해야 한다.
  - 자바스크립트의 선언순서, 위치를 변경함으로써 극복 가능하거나, 매우 짧아질 수 있다.(성능을 위해 `</body>` 요소 앞에 자바스크립트를 위치시키곤 하는데 이를 `<head>` 안으로 위치를 변경해 본다.)
  - FOUC를 유발하는 구역을 숨겼다가 문서의 스타일이나 스크립트가 모두 적용되면 보여준다.

  > https://webdir.tistory.com/416

* ARIA와 screenreader에 대해 설명해주세요. 또 접근성을 지원하는 웹사이트를 어떻게 만드는지에 대해도 설명해주세요.

  ARIA는 (Accessible Rich Internet Applications) 즉 웹 어플리케이션을 작성할 때 장애인을 위한 접근성 향상 방법을 정의한것.
  screenreader는 시각장애인이 컴퓨터를 사용할 때 나타나는 정보들을 음성으로 출력해주는 프로그램이다.

  추가적인 사항은? [여기에서](https://support.office.com/ko-kr/article/sharepoint-online%EC%97%90%EC%84%9C-%EC%A0%91%EA%B7%BC%EC%84%B1-%EB%86%92%EC%9D%80-%EC%82%AC%EC%9D%B4%ED%8A%B8%EB%A5%BC-%EB%A7%8C%EB%93%A4%EA%B8%B0-%EC%9C%84%ED%95%9C-%EB%A6%AC%EC%86%8C%EC%8A%A4-c492ce71-349a-4495-8d8f-1d89bd4adc63)

- CSS 애니메이션과 JavaScript 애니메이션의 차이점에 관해 설명해주세요.

  자바스크립트는 명령형 언어이기 때문에 세밀한 조정이 가능한 것이 장점이고 CSS 애니메이션은 선언형 언어로써 진입장벽이 낮고 또한 브라우저의 메인쓰레드가 아닌 컴포지트라는 별도의 쓰레드에서 구현되기 때문에 GPU의 백 버퍼에서 처리되게 되므로 성능향상에 도움을 줄 수 있습니다.

  단. CSS 애니메이션의 경우 컴포지팅에 영향을 주는 속성 즉 opacity, transform 만 이용하는 것이 좋습니다. left, top 등의 레이아웃에 영향을 주는 속성일 경우 오히려 성능 저하를 일으킬 수 있습니다.

  UI 요소 상태 전환과 같은 간단한 ‘원샷(one-shot)’ 전환에 CSS 애니메이션을 사용합니다.
  바운스, 중지, 일시 중지, 되감기 또는 감속과 같은 고급 효과를 원할 경우에 자바스크립트 애니메이션을 사용합니다.
  자바스크립트로 애니메이션을 만드는 경우, 자신에게 익숙한 Web Animations API 또는 최신 프레임워크를 사용합니다.

  **속도 빠른 순서대로** : velocity.js > css 애니메이션 > jquery 애니메이션

  velocity.js, GSAP 등은 구글이나 어도비 같은 회사들이 모바일 페이지에서 최적화된 애니메이션을 위해 사용하는 라이브러리

  jquery 애니메이션이 느린 이유는 애초에 jquery 가 성능에 초점을 두지 않았기 때문
  jquery는 레이아웃 스레싱이나 가비지 콜렉션 트리거가 발생하기도 함

  출처 1 : https://futurists.tistory.com/60

  출처 2 : https://cyberx.tistory.com/133

* CORS는 무엇의 약자이고 어떤 문제에 대해서 언급하는 것인가요?

  CORS는 Cross Origin Resource Sharing으로 다른 도메인에서 리소스를 공유할 수 있음을 의미합니다. 기본적으로 스크립트는 Same Origin Policy에 의해 HTTP Request가 불가능하나 CORS를 허용하게 된다면 다른 도메인으로 HTTP Request가 가능해진다는 뜻이다. 이를 해결하기 위해선 여러가지 방법이 있는데, JSONP방식을 사용하거나 서버측에서 Access control을 허용하도록 설정해주면 된다.

  좀 더 자세히 : https://futurists.tistory.com/60

---

## HTML 관련 질문

- `doctype`이 무엇을 하는 것인가요?

  **DOCTYPE**은 **document type**의 약어입니다.
  **DOCTYPE**은 항상 **DTD(Document Type Definition)**와 관련됩니다.

  **DTD**는 특정 문서가 어떻게 구성되어야 하는지 정의합니다(예시: `button`은 `span`을 포함할 수 있지만, `div`는 그럴 수 없다.), 반면, **DOCTYPE**은 문서가 _대략_ 존중할만한 **DTD**를 선언합니다. (예시: 이 문서는 HTML DTD를 존중한다.)

  웹 페이지의는 DOCTYPE 선언이 필요합니다. 유저 에이전트에게 문서가 존중하는 HTML 사양의 버전을 알리는데 사용됩니다.
  유저 에이전트가 올바른 DOCTYPE을 인식하면, 문서를 읽는데에 DOCTYPE과 일치하는 **no-quirks mode**를 트리거합니다.
  유저 에이전트가 올바른 DOCTYPE을 인식하지 못하면, **quirks mode**를 트리거합니다.

  HTML5 표준에 대한 DOCTYPE 선언은 ``입니다.

  ###### 참고자료

  - https://html.spec.whatwg.org/multipage/syntax.html#the-doctype
  - https://html.spec.whatwg.org/multipage/xhtml.html
  - https://quirks.spec.whatwg.org/

* 표준모드(standards mode)와 쿽스모드(quirks mode)의 다른 점은 무엇인가요?

  웹 페이지의 렌더링 방식에는 **표준 모드(Standards mode)**와 **관용 모드(Quirks mode)**라는 두 가지 렌더링 방식이 있습니다. 이를 이해하고 DOCTYPE의 중요성을 깨닭게 되길 바랍니다.

  - 표준모드 : 모든 표준이 엄격하게 지켜진다.
  - 관용모드 : 브라우저가 구버전 브라우저의 렌더링을 흉내냄으로써 기존의 비표준 기능도 허용된다.

  **표준 모드 선택**

  DOCTYPE이 지정된 모든 HTML 문서는 윈도우용 IE6 이상 버전을 포함한 모든 브라우저에서 표준 모드로 렌더링됩니다. 극 소수의 예외적인 경우를 제외하고는 표준 모드를 사용해야 합니다.

  ![img](https://t1.daumcdn.net/cfile/tistory/244C6D48552E5FCE0C)

  IE6 이상 버전에서 관용모드를 사용하면 사실 윈도우용 IE5.5와 똑같이 렌더링되는데 이는 기술적으로 엄청난 퇴보입니다. 나머지 브라우저에서는 관용 모드를 사용하면 IE5.5나 다른 브라우저와는 다르게 렌더링됩니다. 관용 모드는 DOCTYPE을 아예 정의하지 않거나 DOCTYPE 정의에 URL을 지정하지 않을때 적용됩니다.

  DOCTYPE 선언 이전에 다른요소가 들어간다면 IE는 관용 모드로 렌더링됨에 주의해야하며, IE6 에서는 XML선언을 넣으면 관용모드로 작동합니다.(``)

  > https://webdir.tistory.com/46 [WEBDIR]

- **XML과 XHTML의 다른 점은 무엇인가요**

  **XHTML**과 **HTML**은 현재 가장 널리 사용되는 웹 문서 규격입니다. 이름에서도 알 수 있듯이 XHTML은 기존에 사용되던 HTML 규격이 가진 문제점을 극복하고, 보다 다양한 분야에 응용될 수 있도록 해주는 여러가지 확장된 기능을 포함하고 있습니다.

  HTML을 **XML** 바탕으로 새롭게 구성(reformulation)한 XHTML은 **CSS**와 함께 최근에 많은 관심을 받고 있는 **‘웹 표준’**의 중요한 요소가 되었습니다. 하지만 XHTML이 XML을 기반으로 만들어졌고, 이 XML을 모든 브라우저가 지원하지 않는다는 현실적인 문제 때문에 XHTML과 HTML이 사실상 큰 차이 없이 사용된다고 주장하는 사람들도 많습니다.

  이런 시각을 다루는 좋은 글이 있어서 번역해서 소개합니다. 내용이 많아서 세 번으로 나눠서 포스팅하려고 하는데 글의 전문성에 비해 제 이해가 많이 부족하고, 원문을 요약한 것이어서 그 내용을 완벽하게 전달하는데 한계가 있으니 감안해서 보시기 바랍니다.

  [Tommy Olsson](http://www.autisticcuckoo.net/)이 쓴 원문은 [Site Point](http://www.sitepoint.com/) 포럼에 올라온 [FAQ About XHTML vs HTML](http://www.sitepoint.com/forums/showthread.php?t=393445)이니 참고하시고, dagger 마크(†)로 시작하는 단락은 원문에는 없는 보충 설명입니다. 이 글의 저작권은 원문의 저작자인 Tommy Olsson과 [Site Point](http://www.sitepoint.com/)에 있으며, 블로그 전체에 적용되는 CCL보다 우선적으로 적용됩니다.

  **XHTML과 HTML의 차이점**

  - XHTML이 XML 문법을 따르므로 HTML과 문법 규칙이 약간 다르다.
  - XHTML을 사용하면 할 수 있으나, HTML로는 불가능한 일이 있다.
  - HTML을 사용하면 할 수 있으나, XHTML로는 불가능한 일이 있다.
  - CSS를 이해하는 방식에 차이가 있다.
  - 클라이언트 쪽의 스크립트(예: 자바 스크립트)를 다루는 방식에 차이가 있다.

  첫 번째로 언급한 문법적인 차이를 다루는 문서는 많기 때문에 자세한 설명을 하지 않겠습니다.

* **XHTML을 이용한 페이지의 한계점은 무엇이 있나요?**

  ##### XHTML을 사용하면 할 수 있으나, HTML로는 불가능한 일

  - CDATA 섹션(`<![CDATA[ … ]]>`) 사용.
    이 섹션 안의 문자들은 태그로 처리되지 않기 때문에 따로 이스케이프(escape) 해 줄 필요가 없다.
  - processing-instruction 사용. 예를 들어 XML 문서에 스타일시트를 연결시킬 수 있다.
    `<?xml-stylesheet type="text/css" href="style.css" media="screen"?>`
  - 다른 XML 이름 영역(namespace)에 있는 요소(element)들을 포함시킬 수 있다.
  - `&apos;` 캐릭터 엔티티(character entity)를 사용할 수 있다.

  ##### HTML을 사용하면 할 수 있으나, XHTML로는 불가능한 일

  - 기존 HTML에서 사용하던 `<!-- … -->` 코멘트로 스타일이나 스크립트의 일부를 주석 처리할 수 없다.
  - 문서를 읽고 있는 도중에는 페이지의 일부를 동적으로 생성할 수 없다(예: `document.write()` 사용).
  - `&nbsp;` 같은 named entity를 사용할 수 없다. 미리 정의된 `<, >, &, "`는 사용 가능.
  - 자바 스크립트에서 `.innerHTML` 속성을 사용할 수 없다.

  > http://blog.wystan.net/2007/05/24/xhtml-vs-html

- `application/xhtml+xml`으로 지정한 페이지에 어떠한 문제가 있나요?

  **XHTML을 `application/xhtml+xml` 타입으로 전송하면 어떤 장점이 있는가?**

  말 그대로 브라우저가 XHTML을 XHTML로 인식한다. XHTML을 사용할 경우에만 얻을 수 있는 장점 때문에 XHTML 문서를 작성했다면 그 장점을 그대로 누릴 수 있다.

  **Content Negotiation 방식을 사용하면 해결되지 않는가?**

  Content Negotiation은 하나의 HTTP 요청에 대해서 두 가지 이상의 자원(문서, 이미지 등)을 준비해서 사용자 에이전트(user agent)에 따라 선택적으로 제공하는 방법이다. 예를 들어서 `application/xtml+xml`을 지원하는 오페라, 파이어폭스, 사파리 브라우저는 XHTML 문서를 `application/xtml+xml` 형태로 제공하고 인터넷 익스플로러가 요청할 때에는 HTML 마크업으로 작성된 HTML 문서를 `text/html` 형태로 보낼 수 있다.

  하지만 이런 방법으로 얻을 수 있는 이점은 다른 컴퓨터 광(geeks)들에게 자신의 능력을 보여주는 것 외에는 전혀 없다. HTML로 변환시킬 수 있는 문서라면 XML만이 지원하는 기능을 전혀 사용하지 않았을 것이기 때문이다. 그렇다면 이름만 다른 두 개의 문서(XHTML, HTML)를 준비하는 것보다 HTML 4.01 스팩을 따르거나 XHTML을 `text/html`로 제공하는 것이 훨씬 쉬운 방법이다.

  Content Type Negotiation은 더 의미가 없다. 같은 문서를 브라우저에 따라 서로 다른 `Content-Type`으로 보내서 얻을 수 있는 이점은 전혀 없다.

  † Content Negotiation을 쉽게 이해하려면 GIF 이미지와 PNG 이미지를 생각하면 됩니다. 동일한 두 가지 이미지를 준비해서 PNG를 제대로 지원하지 않는 인터넷 익스플로러 6.0에게만 GIF 이미지를 전송하는 방법이지요. 자세한 설명은 Content Negotiation에 관한 [위키피디아 문서](http://en.wikipedia.org/wiki/Content_negotiation)를 참고하세요.

  Content Type Negotiation은 모든 요청에 대해 동일한 내용(content)을 전송하면서 HTTP 헤더 정보만 달리하는 것을 말합니다. 동일한 문서가 XHTML도 되고, HTML도 되는 방식입니다.

  **인터넷 익스플로러에서 XHTML을 사용할 수 있는가?**

  불가능하다. 익스플로러가 `application/xhtml+xml` MIME 타입을 지원하지 않으므로 이런 헤더 정보를 받게 되면 해당 페이지를 다운로드하려고 한다. 레지스트리를 변경해서(hack) 이 MIME 타입을 인식하도록 할 수는 있지만 그렇다고 해도 해당 문서는 여전히 HTML로 취급된다.

  XHTML의 XML 기능이 필요하다면 문서를 `application/xml`로 제공할 수 있다. 인터넷 익스플로러도 이 MIME 타입을 지원하지만 XHTML의 이름 영역(namespace)를 사용할 수 없으므로 해당 문서는 보통의 XML 문서로 인식된다. 따라서 스타일시트가 기본적으로 적용되지 않으므로, 모든 요소에 대한 스타일을 전부 지정해줘야 한다. 예를 들어서 모든 블록 레벨의 요소들에 `display: block` 속성을 지정해야 한다.

  물론 XHTML을 `text/html`로 제공할 수 있다. 하지만 앞서 길게 설명했던 것처럼 브라우저는 그 XHTML 문서를 문법 오류가 있는 HTML 문서로 인식한다.

  † 여기서 말하는 문법 오류는 닫는 태그 앞에 공백과 슬래시 기호가 있는 것을 의미합니다. 예를 들어서 `` 태그 같은 것이지요.

  **인터넷 익스플로러 7은 XHTML을 제대로 지원하는가?**

  그렇지 않다.

  > http://blog.wystan.net/2007/05/24/xhtml-mime-type

* 다국어가 포함된 페이지는 어떤 방식으로 제공하나요?

  이 질문은 다소 모호합니다. 여러 언어로 제공되는 내용의 페이지를 제공하는 방법에 대한, 가장 일반적인 경우에 대해 묻고 있다고 가정합니다. 하지만 페이지 내의 내용은 하나의 일관된 언어로만 표시되어야합니다.

  HTTP 요청을 서버에 보내면, 대개 요청하는 유저 에이전트가 `Accept-Language` 헤더와 같은 기본 언어 설정에 대한 정보를 보냅니다. 그 다음 서버는 이 정보를 사용하여 해당 언어가 제공 가능한 경우, 해당 언어 버전의 문서를 반환할 수 있습니다. 반환된 HTML 문서는 `<html lang="en">...</html>`과 같이 `<html>` 태그에 `lang` 속성을 선언해야 합니다.

  백엔드에서, HTML 마크업은 YML 또는 JSON 형식으로 저장된 특정 언어에 대한 `i18n` placeholder와 내용을 포함합니다. 그 다음 서버는 일반적으로 백엔드 프레임워크의 도움을 받아 특정 언어로 HTML 페이지를 동적 생성합니다.

  ###### 참고자료

  - https://www.w3.org/International/getting-started/language

- **다국어 페이지를 제공하는 여러 방법에 관해 설명해주세요.**

  - HTML에 `lang` 속성을 사용합니다.
  - 사용자를 그들의 모국어로 안내합니다 - 사용자가 번거롭지 않도록 쉽게 국가/언어를 변경할 수 있도록 합니다.
  - 텍스트를 포함한 이미지를 사용하는 것은 확장가능한 접근이 아닙니다 - 이미지에 텍스트를 배치하는 것은 잘 보이고 시스템 글꼴이 아닌 글꼴을 모든 컴퓨터에 표시하는데 여전히 널리 사용되는 방법입니다. 그러나 이미지에 텍스트를 번역하려면, 텍스트 문자열에 각 언어에 대해 만들어진 별도 이미지가 필요합니다. 이 같은 대체 방식이 늘어나면 금방 통제가 어려워집니다.
  - 단어/문장 길이 제한 - 일부 언어는 다른 언어로 작성될 때 더 길어질 수도 있습니다. 디자인에 레이아웃이나 오버 플로우 문제 발생에 주의하세요. 디자인에 필요한 텍스트의 양을 정하거나, 디자인이 꺠질 수 있는 디자인은 하지 않도록 하는 것이 가장 좋습니다. 문자 수 제한은 제목, 레이블, 버튼과 같은 항목에서 사용됩니다. 본문이나 댓글과 같이 자유롭게 흐르는 텍스트에 대해서는 문제가 되지 않습니다.
  - 색상이 어떻게 이해될지에 대해 주의 깊게보세요 - 색상은 언어와 문화에 따라 다르게 인식됩니다. 적절한 색상을 사용하여 디자인해야 합니다.
  - 날짜와 통화 형식 - 날짜는 종종 다른 방식으로 표현됩니다. 예) 미국의 "May 31, 2012" vs. 유럽의 "31 May 2012".
  - 번역된 문자열을 연결하지 않습니다 - `"오늘의 날짜는 " + date + "입니다"` 와 같은 것은 하지마세요. 단어의 순서가 다른 언어에서는 문자가 망가지게됩니다. 대신 각 언어에 대한 매개변수와 함께 템플릿 스트링을 사용하세요. 예를 들면, 영어와 한국어로된 다음 두 문장을 보세요. `I will travel on {% date %}`, `나는 {% date %}에 여행 갈거야`. 변수의 위치는 언어의 문법에 따라 달라집니다.
  - 언어를 읽는 방향 - 영어는 왼쪽에서 오른쪽으로, 위에서 아래로 읽지만, 전통적인 일본어는 위에서 아래로, 오른쪽에서 왼쪽으로 읽습니다.

  ###### 참고자료

  - https://www.quora.com/What-kind-of-things-one-should-be-wary-of-when-designing-or-developing-for-multilingual-sites

* **`data-`속성은 무엇을 하는 것인가요? 사용했을 때 이점은 무엇인가요?**

  JavaScript 프레임워크가 인기있기 전에, 프론트엔드 개발자는 비표준 속성, DOM 추가 프로퍼티 등의 조작없이, DOM 자체에 추가적인 데이터를 저장하기 위해 `data-`속성을 사용했었습니다. 이는 적절한 속성이나 요소가 없는 페이지나 애플리케이션에 사용자정의 데이터를 비공개로 저장하기 위한 것입니다.

  요즘에는, `data-`속성을 사용하는 것을 권장하지 않습니다. 그 이유 중 하나는 사용자가 브라우저의 inspect 기능를 사용하여 데이터 속성을 쉽게 수정할 수 있다는 것입니다. 데이터 모델은 JavaScript 자체에 더 잘 저장되며, 라이브러리나 프레임워크의 데이터 바인딩을 통해 DOM을 업데이트된 상태로 유지하는 것이 더 낫습니다.

  ###### 참고자료

  - http://html5doctor.com/html5-custom-data-attributes/
  - https://www.w3.org/TR/html5/dom.html#embedding-custom-non-visible-data-with-the-data-*-attributes

- **HTML5를 오픈 웹 플랫폼(open web platform)으로 생각해본다면, 어떤 것들로 구성돼 있을까요?**

  - 의미 - 콘텐츠를 보다 더 정확하게 설명할 수 있도록 허용합니다.
  - 연결 - 새롭고 혁신적인 방법으로 서버와 통신할 수 있도록 허용합니다.
  - 오프라인과 저장소 - 웹 페이지가 클라이언트 측에서 데이터를 로컬로 저장하여, 오프라인에서보다 효율적으로 작동하도록 허용합니다.
  - 멀티미디어 - 개방형 웹에서 비디오와 오디오를 일급으로 만듭니다.
  - 2D/3D 그래픽과 효과 - 훨씬 다양한 프레젠테이션 옵션을 허용합니다.
  - 성능과 통합 - 컴퓨터 하드웨어의 성능 최적화와 개선으로 더 나은 사용을 제공합니다.
  - 장치 접근 - 다양한 입출력 장치의 사용을 허용합니다.
  - 스타일링 - 사용자가 더 세련된 테마를 사용하게 합니다.

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5

* **`쿠키(Cookies)`와 `세션저장소(sessionStorage)`와 `로컬저장소(localStorage)`의 차이점을 설명해주세요.**

  위 세 가지 기술은 모두 클라이언트 측에서 값을 저장하는 key-value 저장소 매커니즘입니다. 모두 문자열로만 값을 저장할 수 있습니다.

  |                                   | `cookie`                                                         | `localStorage` | `sessionStorage` |
  | --------------------------------- | ---------------------------------------------------------------- | -------------- | ---------------- |
  | 생성자                            | 클라이언트나 서버. 서버는 `Set-Cookie` 헤더를 사용할 수 있습니다 | 클라이언트     | 클라이언트       |
  | 만료                              | 수동으로 설정                                                    | 영구적         | 탭을 닫을 때     |
  | 브라우저 세션 전체에서 지속       | 만료 설정 여부에 따라 다름                                       | O              | X                |
  | 모든 HTTP 요청과 함께 서버로 보냄 | 쿠키는 `Cookie` 헤더를 통해 자동 전송됨                          | X              | X                |
  | 용량 (도메인당)                   | 4kb                                                              | 5MB            | 5MB              |
  | 접근성                            | 모든 윈도우                                                      | 모든 윈도우    | 같은 탭          |

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies
  - http://tutorial.techaltum.com/local-and-session-storage.html

- **`<script>, <script async>`와 `<script defer>`의 차이점에 관해 설명해주세요.**

  - `<script>` - HTML 파싱이 중단되고, 스크립트를 즉시 가져오고 실행되며, 스크립트 실행 후 HTML 파싱이 다시 시작됩니다.
  - `<script async>` - 이 스크립트는 HTML 파싱과 병렬적으로 가져오며, 가능할 때 즉시 실행됩니다(아마 HTML 파싱이 끝나기 전). 스크립트가 페이지의 다른 스크립트들과 독립적인 경우 `async`를 사용하세요. 예) analytics.
  - `<script defer>` - 이 스크립트는 HTML 파싱과 병렬적으로 가져오지만, 페이지 파싱이 끝나면 실행됩니다. 이 것이 여러개 있는 경우, 각 스크립트는 페이지에 등장한 순서대로 실행됩니다. 스크립트가 완전히 파싱된 DOM에 의존되는 경우 `defer` 속성은 스크립트를 실행하기 전에 HTML이 완전히 파싱되도록 하는데 유용합니다. `<body>`의 끝부분에 일반 `<script>`를 두는 것과 별 차이가 없습니다. `defer` 스크립트는 `document.write`를 포함하면 안됩니다.

  주의: `src` 속성이 없는 스크립트 태그는 `async` 와 `defer` 속성이 무시됩니다.

  ###### 참고자료

  - http://www.growingwiththeweb.com/2014/02/async-vs-defer-attributes.html
  - https://stackoverflow.com/questions/10808109/script-tag-async-defer
  - https://bitsofco.de/async-vs-defer/

* **CSS`<link>`를 `<head></head>`사이에 쓰는 것과 JS`<script>`를 `<body></body>`뒤에 사용하는 것은 좋은 사용법일까요? 어디에 배치하는 게 좋을까요?**

  **`<head>` 안에 `<link>`를 넣는 이유**

  `를` 안에 넣는 것은 최적화된 웹사이트를 구출할 때 적절한 명세의 일부입니다. 페이지가 처음로드되면 HTML과 CSS가 동시에 파싱됩니다. HTML은 DOM(Document Object Model)을 만들고 CSS는 CSSOM (CSS Object Model)을 만듭니다. 두 가지 모두 웹사이트에서 시각적인 부분을 만드는데 필요하므로, 빠른 "first meaningful paint"를 가능하게 합니다. 이 점진적 렌더링은 사이트의 성능 점수에서 측정되는 사이트 최적화의 범주입니다. 문서 최하단에 스타일시트를 두는 것은 많은 브라우저에서 점진적 렌더링을 금지하게 되는 것입니다. 몇몇 브라우저는 스타일이 변경되면 페이지의 요소를 다시 그리는 것을 피하기 위해 렌더링을 차단합니다. 그렇게되면 사용자는 빈 하얀 페이지를 보게됩니다.

  그 외에도 상단에 배치하면 페이지가 점진적으로 렌더링되기 때문에 UX가 향상됩니다. 문서 맨 아래에 CSS 를 두는 것은 Internet Explorer 를 비롯한 많은 브라우저에서 점진적 렌더링을 금지시키는 것입니다. 몇몇 브라우저는 스타일이 변경되면 페이지의 요소를 다시 그리지 않아도 되도록 렌더링을 차단합니다. 사용자는 빈 하얀 페이지에서 멈추게 됩니다. 또한 스타일이 없는 내용이 잠깐 보이는 것을 방지합니다. 다른 경우에는 스타일되지 않은 내용이 깜빡일 수 있습니다(flashes of unstyled content: FOUC).

  **`</body>` 직전에 `<script>`를 넣는 이유**

  `<scritp>`는 다운로드되고 실행되는 동안 HTML 파싱을 차단합니다. 스크립트를 맨 아래에 두면 HTML을 먼저 파싱하여 사용자에게 표시할 수 있습니다.

  스크립트에 `document.write()`가 있을 때는 `<script>`를 아래쪽에 두는 것이 예외적일 수 있습니다만, 요즘은 `document.write()`를 사용하지 않는 것이 좋습니다. 또한, `<script>`를 맨 아래에 두면, 브라우저가 전체 문서가 파싱될 때까지 스크립트 다운로드를 시작할 수 없다는 것을 의미합니다. 이렇게하면 DOM 요소를 조작해야하는 코드가 오류를 발생시키지 않고 전체 스크립트를 중지시키지 않습니다. `<head>`에 `<script>`를 넣어야하는 경우, `defer` 속성을 사용하세요. HTML을 파싱한 후에 스크립트를 다운로드하고 실행하는 것과 같은 효과가 있습니다.

  ###### 참고자료

  - https://developer.yahoo.com/performance/rules.html#css_top
  - https://www.techrepublic.com/blog/web-designer/how-to-prevent-flash-of-unstyled-content-on-your-websites/
  - https://developers.google.com/web/fundamentals/performance/critical-rendering-path/

- **Progressive rendering이란 무엇인가요?**

  프로그레시브 렌더링이란 콘텐츠를 가능한한 빠르게 표시하기 위해 웹 페이지의 성능을 향상시키는 데 사용되는 기술입니다. (특히, 인식되는 로딩 시간을 향상시킵니다)

  예전에는 광대역 인터넷을 사용하기도 했지만 불안정한 모바일 데이터 연결이 점점 인기를 끌면서 최근 개발에 있어서도 여전히 유용합니다!

  관련 기술 예시:

  - 이미지 지연 로딩 - 페이지의 이미지를 한꺼번에 로딩하지 않습니다. JavaScript를 사용하여 사용자가 이미지를 표시하는 페이지 부분으로 스크롤 할 때 이미지를 로드 할 수 있습니다.
  - 보이는 콘텐츠의 우선순위 설정 (또는 스크롤 없이 볼 수 있는 렌더링) - 가능한 한 빨리 표시하기 위해 사용자 브라우저에서 렌더링될 페이지에 필요한 최소한의 CSS/콘텐츠/스크립트 만 포함하면 `deferred` 스크립트를 사용하거나 `DOMContentLoaded`/`load` 이벤트를 사용하여 다른 리소스와 내용을 로드할 수 있습니다.
  - 비동기 HTML 프래그먼트 - 페이지의 백엔드에서 HTML 페이지의 일부를 브라우저로 가져옵니다. 이 기술에 대한 자세한 내용은 [여기](http://www.ebaytechblog.com/2014/12/08/async-fragments-rediscovering-progressive-html-rendering-with-marko/)에서 찾을 수 있습니다.

  ###### 참고자료

  - https://stackoverflow.com/questions/33651166/what-is-progressive-rendering
  - http://www.ebaytechblog.com/2014/12/08/async-fragments-rediscovering-progressive-html-rendering-with-marko/

* **이미지 태그에 `srcset` 속성을 사용하는 이유는 무엇인가요? 브라우저가 이 속성을 가진 콘텐츠를 평가할 때 사용하는 과정을 설명해보세요.**

  기기의 디스플레이 너비에 따라 다른 이미지를 사용자에게 제공하려는 경우 `srcset` 속성을 사용합니다 - 레티나 디스플레이를 통해 장치에 고품질 이미지를 제공하여 사용자 경험을 향상시키고, 저해상도 이미지를 저사양 기기에 제공하여 성능을 높이고 데이터 낭비를 줄입니다. (왜냐하면 더 큰 이미지를 제공하는 것은 눈에 보일 정도의 차이가 없기 때문). 예를 들면: `<img srcset="small.jpg 500w, medium.jpg 1000w, large.jpg 2000w" src="..." alt="">`는 클라이언트의 해상도에 따라 브라우저에 small, medium, large `.jpg` 그래픽을 표시하도록 지시합니다. 첫 번째 값은 이미지 이름이고 두 번째 값은 픽셀 단위의 이미지 너비입니다. 320px 너비의 경우, 다음과 같은 계산을 따릅니다

  - 500 / 320 = 1.5625
  - 1000 / 320 = 3.125
  - 2000 / 320 = 6.25

  클라이언트의 해상도가 1x 일 경우, 1.5625가 가장 가깝고 `small.jpg`에 해당하는 `500w`가 브라우저에 의해 선택됩니다.

  해상도가 레티나 (2x)인 경우 브라우저는 최소값에서 가장 위로 가까운 해상도를 사용합니다. 500w (1.5625)는 1보다 크고 이미지가 보기 좋지 않을 수 있기 때문에 선택하지 않는다는 것을 의미합니다. 그래서 브라우저는 계산 결과 비율값이 2에 가까운 1000w (3.125) 이미지를 선택합니다.

  `srcset`는 데스크탑 디스플레이처럼 거대한 이미지를 필요로하지 않기 때문에 화면 장치를 좁히는 작은 이미지 파일을 제공하고자하는 문제를 해결합니다.

  `srcset`는 화면이 작은 기기에서 데스크탑 디스플레이처럼 큰 이미지가 필요하지 않기 때문에 작은 이미지 파일을 제공하는 문제를 해결합니다 — 또한 선택적으로 고해상도/저해상도 화면에 다른 해상도 이미지를 제공할 수도 있습니다.

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images
  - https://css-tricks.com/responsive-images-youre-just-changing-resolutions-use-srcset/

- **HTML templating language를 사용해 본 경험이 있나요?**

  사용해 본적은 없지만 알고있다.

  Pug (formerly Jade), ERB, Slim, Handlebars, Jinja, Liquid 등이 있다.

  `Template Engine` 이란 템플릿 양식과 특정 데이터 모델에 따른 입력 자료를 합성하여 결과 문서를 출력하는 소프트웨어(또는 소프트웨어 컴포넌트)를 말한다.

  그 중 **웹 템플릿 엔진(web template engine)**이란 웹 문서가 출력되는 템플릿 엔진을 말한다. 이는 **웹 템플릿(web templates)**과 **웹 컨텐츠 정보(content information)**를 처리하기 위해 설계된 소프트웨어이다. 웹 템블릿 엔진은 vie w code(html)와 data logic code(db connection)를 분리해주는 기능을 한다.

  ![image](https://user-images.githubusercontent.com/42582516/83379772-4cec9e80-a417-11ea-919b-c3be64066d6a.png)

  템플릿 엔진의 종류는 **레이아웃 템플릿 엔진**과 **텍스트 템플릿 엔진**으로 나눌 수 있다.

  - 레이아웃 템플릿 엔진 : 중복하는 `include` 코드를 사용하지 않고도 지정된 페이지 레이아웃에 따라 페이지 타일을 조합하여 완전한 페이지로 만들어줌.

    > Ex) Apache Tiles, Sitemash

  - 텍스트 템플릿 엔진 : 템플릿 양식에 적절한 특정 데이터를 넣어 결과 문서를 출력한다.

    > Ex) Freemarker, Thymeleaf, JSP(Java Server Pages) 등

  둘은 역할이 다르며 섞어서 사용하는 것이지 서로 배타적인 것이 아니다.

  **서버 사이드 템플릿 엔진** vs **클라이언트 사이드 템플릿 엔진**

  - **Server** Side Template Engine : 서버에서 DB 혹은 API에서 가져온 데이터를 미리 정의된 Template에 넣어 html 을 그려서 클라이언트에 전달해주는 역할을 한다.

    HTML 코드에서 고정적으로 사용되는 부분은 템플릿으로 만들어두고 동적으로 생성되는 부분만 템플릿 특정 장소에 끼워넣는 방식으로 동작할 수 있도록 해준다.

    ![image](https://user-images.githubusercontent.com/42582516/83380427-e5375300-a418-11ea-9a80-6b63a63360cd.png)

    과정

    1. 클라이언트의 요청을 받아서
    2. 필요한 데이터(DB에서 가져오거나 API에서 가져오거나) 가져온다.
    3. 미리 정의된 Template에 해당 데이터를 적절하게 넣는다.
    4. 서버에서 HTML(데이터가 반영된 Template)을 그린다
    5. 해당 HTML을 클라이언트에 전달한다.

  - **Client** Side Template engine

    html 형태로 코드를 작성할 수 있으며, 동적으로 DOM을 그리게 해주는 역할을 한다.

    즉, 데이터 받아서 DOM 객체에 동적으로 그려주는 프로세스를 담당한다.

    예를 들어 웹 페이지에서 여러 카테고리 중 탭을 선택할 때만다 같은 형식의 프레임에 내용만 바뀌어 변경되는 것을 볼 수 있다. 이런 공통적인 프레임을 미리 제작한 'template'이라고 부른다. 클라이언트에서는 이런 template을 매번 입력하거나 바꿀 수 없으므로 script 타입을 template으로 미리 만들어 사용한다. (안의 내용은 replace를 사용하여 바꾼다.)

    ![image](https://user-images.githubusercontent.com/42582516/83380769-c6858c00-a419-11ea-8f20-f9672e43dc81.png)

    과정

    1. 클라이언트에서 공통적인 프레임을 미리 template으로 만든다
    2. 서버에서 필요한 데이터를 받는다.
    3. 데이터를 template을 적절한 위치에 replace하고 DOM 객체에 동적으로 그려준다.

    필요한 경우

    1. Javascript 라이브러리로 랜더링이 끝난뒤 (즉, HTML Dom이 다 그려진 뒤)에 서버 통신 없이 화면 변경이 필요한 경우
    2. 계속해서 페이지를 이동하여 서버 쪽으로 호출이 발생한다면 서버 사이드 템플릿 엔진을 이용하면 되는데, 단일 화면에서 특정 이벤트에 따라 화면이 계속 변경되어야 하는 경우는 javascript로 html을 렌더링하는 경우가 많다.
    3. 이렇게 단일 화면에서의 화면 변경에서는 서버 쪽을 사용하지 않은 화면을 그리 위해 javascript 안에 html 코드를 작성해야하는데, 이때 클라이언트 사이드 템플릿 엔진을 사용하지 않고 아래와 같이 javascript로 html을 ㄹ헨더링하는 경우에는 여러 문제가 있음 => html 코드의 오타를 찾기 어렵다, 렌더링 해야 할 코드 늘어나면 늘어날수록 수정하기 어려워진다.

  **SprintMVC 템플릿 엔진** vs **Sprint boot 템플릿 엔진**

  Java Object에서 데이터를 생성하여 Template에 넣어주면 템플릿 엔진에서 Template에 맞게 변환하여 html 파일을 생성하는 역할을 한다.

  **템플릿 엔진(Template Engine)의 필요성**

  1. 많은 코드를 줄일 수 있다. : 대부분의 Template Engine은 기존의 HTML에 비해서 간단한 문법을 사용한다.
  2. 재사용성이 높다. : 웹페이지 혹은 웹앱을 만들 때 똑같은 디자인의 페이지에 보이는 데이터만 바뀌는 경우가 굉장히 많다.
  3. 유지보수에 용이하다. : 하나의 Template을 만들어 여러 페이지를 렌더링하는 작업에는 또 다른 이점이 있다.

  > https://gmlwjd9405.github.io/2018/12/21/template-engine.html

### References

- https://velog.io/@chris/front-end-interview-handbook-html

---
