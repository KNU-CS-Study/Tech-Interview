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

## CSS 관련 질문

- **class와 id의 차이점에 관해서 설명해주세요.**

  id 선택자와 class 선택자는 특정 요소를 대상으로 스타일을 적용하기 위한 것입니다. 예를 들어 id와 class를 사용하면 모든 <p>요소가 아닌 특정한 <p>요소에만 스타일을 적용할 수 있습니다.

  id 선택자와 class 선택자의 차이는 문서 안의 '복수'의 요소에 스타일을 적용하는 것인가 아니면 '유일'한 요소에 스타일을 적용하는 것인가입니다. 결론적으로 말하면 id는 '유일'한 요소에 적용, class는 '복수'의 요소에 적용할 수 있습니다.

  - id : '유일'한 요소에 스타일을 적용
  - class : '복수'의 요소에 스타일을 적용

  **id 선택자**

  id 선택자는 문서 안에 있는 단 하나의 요소에 스타일을 적용하는 경우에 사용합니다. 선택자에 샤프(#)와 id명(임의의 이름)을 붙여 식별합니다.

  **class 선택자**

  class 선택자는 문서 안 복수의 요소에 스타일을 적용하는 경우에 사용합니다. 요소명에 피리어드(.)와 class명(임의의 이름)을 붙여 구별합니다.

  **id와 class의 차이점을 다시 정리해보면..**

  - 하나의 id는 한 문서에서 한 번만 사용이 가능합니다.
  - 하나의 class는 한 문서에서 여러 번 사용이 가능합니다.
  - id의 속성이 class의 속성보다 우선 순위가 높습니다.
  - 따라서 id의 속성은 해당 요소에 부여된 class 속성에 관계 없이 작동합니다.

  > https://ohknow.tistory.com/35 [오늘의 잡지식 Oh~Know~]

* **div와 span의 차이**

  div 요소는 블록(block) 레벨 요소이며 인라인(inline) 요소와 텍스트를 포함하고 다시금 블록 레벨 요소를 포함할 수 있습니다. 한편 span 요소는 인라인(inline) 요소이며 인라인 요소와 텍스트를 포함하지만 블록 레벨 요소를 포함할 수는 없습니다. 따라서 div 요소는 블록 레벨 요소, span 요소는 인라인 요소나 텍스트의 그룹화를 위해 사용합니다.

  - div : 블록(block) 요소
  - span : 인라인(inine) 요소

  앞의 그림을 보면 div와 div는 줄 바꿈이 생기고, span과 span 사이에는 줄 바꿈이 생기지 않는 것을 볼 수 있습니다. div는 전체적인 레이아웃을 잡을 때, span은 텍스트 스타일 등 특정 부분에 스타일을 지정할 때 사용할 수 있습니다.

  > https://ohknow.tistory.com/35 [오늘의 잡지식 Oh~Know~]

- **UI와 UX의 차이점**

  디바이스와 이용자간의 매개체가 UI, 매개 후 결과는 UX
  \----------------------------------------------
  UI(user interface)
  사용자가 앱을 사용할 때 마주하는 디자인, 레이아웃, 기술적인 부분으로 다양한 사용자가 사용할 수 있도록 보편성을 지녀야한다.

  UX(user experience)
  앱을 주로 사용하는 사용자들의 경험들을 분석하여 더 편하고 효율적인 방향으로 프로세스가 진행될 수 있도록 하는 과정, 결과이다.

* **CSS 선택자의 특정성은 무엇이며 어떻게 작동하나요?**

  브라우저는 CSS 규칙의 특정성에 따라 요소에 표시할 스타일을 결정합니다. 브라우저는 이미 특정 요소와 일치하는 규칙을 결정했다고 가정합니다. 일치하는 규칙들 가운데, 네개의 쉼표로 구분된 값 `a, b, c, d`는 다음을 기반으로 각 규칙에 대해 계산됩니다.

  1. `a`는 인라인 스타일이 사용되고 있는지 여부입니다. 속성의 선언이 요소의 인라인 스타일이면 `a`는 1이고, 그렇지 않으면 0입니다.
  2. `b`는 ID 셀렉터의 수입니다.
  3. `c`는 클래스, 속성, 가상 클래스 선택자의 수입니다.
  4. `d`는 태그, 가상 요소 선택자의 수입니다.

  결과적인 특정성은 점수가 아니라, 컬럼마다 비교할 수 있는 값들의 행렬입니다. 선택자를 비교하여 가장 높은 특정성을 갖는 항목을 결정할 때, 왼쪽에서 오른쪽 순으로 각 열의 가장 높은 값을 비교합니다. 따라서 `b`열의 값은 `c`와 `d`열에 있는 값을 무시합니다. 따라서 `0,1,0,0`의 특정성은 `0,0,10,10`중 하나보다 큽니다.

  동등한 특정성의 경우: 가장 마지막 규칙이 중요한 규칙입니다. 스타일시트에 동일한 규칙을 두 번 작성한 경우(내부나 외부에 관계없이) 스타일시트의 하위 규칙이 스타일될 요소에 더 가까우므로 더 구체적으로 적용됩니다.

  저라면, 필요하다면 쉽게 재정의할 수 있도록 낮은 특정성 규칙들을 작성할 것입니다. CSS UI 컴포넌트 라이브러리 코드를 작성할 때, 라이브러리 사용자가 `!important`를 사용하거나 특정성을 높이기 위해 지나치게 복잡한 CSS 규칙을 사용하지 않고도 이를 재정의할 수 있도록 특정성을 낮게 하는 것이 중요합니다.

  ###### 참고자료

  - https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/
  - https://www.sitepoint.com/web-foundations/specificity/

- **Resetting과 Normalizing CSS의 차이점은 무엇인가요? 당신은 무엇을 선택할 것이며, 그 이유는 무엇인가요?**

  - **Resetting** - Resetting은 요소의 모든 기본 브라우저 스타일을 제거하기 위한 것입니다. 예: `margin`, `padding`, `font-size`는 같은 값으로 재설정됩니다. 일반적인 타이포그래피 요소에 대한 스타일을 재 선언해야합니다.
  - **Normalizing** - Normalizing는 "모든 스타일을 제거"하는 것이 아니라 유용한 기본 스타일을 보존합니다. 또한 일반적인 브라우저 종속성에 대한 버그를 수정합니다.

  필자는 저만의 스타일링을 많이 해야 하고 보존할 기본 스타일이 필요하지 않도록 매우 커스터마이징되었거나 자유로운 사이트 디자인해야할 때 리셋을 선택합니다.

  ###### 참고자료

  - https://stackoverflow.com/questions/6887336/what-is-the-difference-between-normalize-css-and-reset-css

* **Floats가 어떻게 동작하는지 설명해주세요.**

  Float는 CSS 위치지정 속성입니다. Float된 요소는 페이지의 흐름의 일부가 되며, 페이지의 흐름에서 제거되는 `position: absolute` 요소와 달리 다른 요소(예: 플로팅 요소 주위로 흐르는 텍스트)의 위치에 영향을 줍니다.

  CSS `clear` 속성은 float 요소에 `left`/`right`/`both`에 위치하도록 사용될 수 있습니다.

  부모 요소에 float 요소만 있으면, 그 높이는 무효가 됩니다. 컨테이너의 float 요소 다음에 있지만 컨테이너가 닫히기 전에 float를 clear하면 해결할 수 있습니다.

  `.clearfix`는 영리한 CSS 가상 선택자 (`:after`)를 사용하여 float를 제거합니다. 상위 클래스에 overflow 를 설정하는 대신 추가 클래스 `clearfix`를 적용합니다. 그 다음 아래 CSS를 적용하세요:

  ```css
  .clearfix:after {
    content: " ";
    visibility: hidden;
    display: block;
    height: 0;
    clear: both;
  }
  ```

  대신, 부모 요소에 `overflow: auto`나 `overflow: hidden` 속성을 주면, 자식 요소 내부에 새로운 블록 포맷 컨텍스트을 설정하고 자식을 포함하도록 확장합니다.

  ###### 참고자료

  - https://css-tricks.com/all-about-floats/

- **`z-index`와 스택 컨텍스트(stacking context)가 어떻게 형성되는지 설명하세요.**

  CSS의 `z-index`속성은 겹치는 요소의 쌓임 순서를 제어합니다. `z-index`는 `position`에 `static`이 아닌 값을 갖는 요소에만 영향을 줍니다.

  `z-index` 값이 없으면 DOM에 나타나는 순서대로 요소가 쌓이게 됩니다(동일한 계층에서 가장 아래의 것이 맨 위에 보여집니다). 정적이지 않은(non-static) 위치지정 요소(및 해당 하위 요소)는 HTML 레이어 구조와 상관없이 기본 정적 위치로 항상 요소 위에 나타납니다.

  스택 컨텍스트(stacking context)는 레이어들을 포함하는 요소입니다. 지역 스택 컨텍스트 내에서, 자식의 `z-index` 값은 문서 루트가 아닌 해당 요소를 기준으로 설정됩니다. 해당 컨텍스트 외부 레이어(예: 지역 스택 컨텍스트의 형제 요소)는 그 사이의 레이어에 올 수 없습니다. 요소 B가 요소 A의 상단에 위치하는 경우, 요소 A의 하위 요소 C는, 요소 C가 요소 B보다 `z-index`가 더 높은 경우에도 요소 B 보다 위에 올 수 없습니다.

  각각의 스택 컨텍스트는 자체적으로 포함되어 있습니다 - 요소의 내용이 쌓인 후에는 전체 요소를 스택 컨텍스트의 쌓인 순서로 고려합니다. 다음 몇몇 CSS 속성, `opacity`가 1보다 작거나, `filter`가 `none`이 이거나, `transform`이 `none`이 아닌 것들이 새로운 스택 컨텍스트를 트리거합니다.

  ###### 참고 자료

  - https://css-tricks.com/almanac/properties/z/z-index/
  - https://philipwalton.com/articles/what-no-one-told-you-about-z-index/

* **BFC(Block Formatting Context)와 그 작동 방식을 설명하세요.**

  BFC(Block Formatting Context)는 블록 박스가 배치된 웹 페이지의 시각적 CSS 렌더링의 일부입니다. float, absolute로 배치된 요소, `inline-blocks`, `table-cells`, `table-caption` 그리고 `visible`(그 값이 viewport에 전파되었을 때는 제외)이 아닌 `overflow`가 있는 요소들이 새로운 Block Formatting Context를 만듭니다.

  BFC는 다음 조건 중 하나 이상을 충족시키는 HTML 박스입니다:

  - `float`의 값이 `none`이 아님.
  - `position`의 값이 `static`도 아니고 `relative`도 아님.
  - `display`의 값이 `table-cell`, `table-caption`, `inline-block`, `flex`, `inline-flex`임.
  - `overflow`의 값이 `visible`이 아님.

  BFC에서 각 박스의 왼쪽 바깥 모서리는 포함하는 블록의 왼쪽 모서리에 닿습니다(right-to-left 포맷에서는, 오른쪽 모서리에 닿음).

  BFC collapse시에 인접한 블록 레벨 박스 사이의 수직 마진. [collapsing margins](https://www.sitepoint.com/web-foundations/collapsing-margins/)에 대해 자세히 읽어보세요.

  ###### 참고 자료

  - https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Block_formatting_context
  - https://www.sitepoint.com/understanding-block-formatting-contexts-in-css/

- **클리어링(Clearing) 기술에는 어떤 것들이 있으며, 어떨 때 어떻게 사용하는 것이 적절한지 설명하세요.**

  - 빈 `div` 방법 - `<div style="clear:both;"></div>`
  - Clearfix 방법 - 위 `.clearfix` 클래스를 참조하세요.
  - `overflow: auto` 또는 `overflow: hidden` 방법 - 부모는 새로운 Block Formatting Context를 설정하고, 확장된 자식을 포함하도록합니다.

  대규모의 프로젝트에서는 유용하게 `.clearfix` 클래스를 만들어 필요한 곳에서 사용합니다. 자식이 부모보다 크기가 경우 `overflow: hidden`은 자식을 모두 보여줄 수 없습니다.

* **CSS 스프라이트(CSS Sprites)를 설명하고, 페이지나 사이트를 어떻게 향상하는지 설명하세요.**

  CSS 스프라이트는 여러 이미지를 하나의 큰 이미지로 결합합니다. 일반적으로 아이콘에 사용되는 기술(Gmail에서 사용)입니다. 구현 방법:

  1. 스프라이트 생성기를 사용하여 여러 이미지를 하나로 묶어 적절한 CSS를 생성합니다.
  2. 각 이미지는 `background-image`, `background-position`, `background-size` 속성이 정의된 해당 CSS 클래스를 갖습니다.
  3. 해당 이미지를 사용하기위해, 요소에 해당 클래스를 추가합니다.

  **장점:**

  - 여러 이미지에 대한 HTTP 요청 수를 줄입니다(스프라이트 시트당 하나의 단일 요청만 필요합니다.) 그러나 HTTP2를 사용하면, 여러 이미지를 로드하는 것이 더 이상 중요하지 않습니다.
  - `:hover`의 상태에서만 나타나는 이미지가 필요할 때, 다운로드되지 않는 이미지를 미리 다운로드하여 깜박임이 보이지 않습니다.

  ###### 참고 자료

  - https://css-tricks.com/css-sprites/

- **Image Replacement를 사용해야 할 때, 선호하는 기술과 언제 사용하는지를 설명해주세요.**
  - 이미지 대체는 시각장애인들이 이미지 요소의 정보를 얻을 수 있도록 하기 위해 screen reader 기가 읽을 수 있도록 넣는 속성, 또 어떤 이유로 이미지가 로드 되지 않았을 때 이미지 대신 볼 수 있는 텍스트를 제공하는 것이다.
  - `img`태그의 경우 `alt` 속성 및 `attr` 속성을 쓴다.
  - background-image의 경우 대체가능한 태그로 이미지에 대한 설명을 쓰고 background-image에 대한 태그를 숨긴다.

* **브라우저 스펙 차이에 따른 스타일링 이슈를 수정하기 위해서 어떻게 접근하나요?**

  - 같은 CSS 속성을 넣어도 다른 디자인으로 표현되거나 레이아웃이 깨질 수 있다.

- **브라우저 별로 스타일이 다른 문제를 어떤 접근 방법으로 해결하나요?**

  - 문제와 그 문제를 일으키는 브라우저를 식별한 후, 해당 브라우저가 사용 중일 때만 로드되는 별도의 스타일 시트를 사용합니다. 하지만 이 방식을 사용하려면 서버사이드 렌더링이 필요합니다.
  - 이미 이러한 스타일링 문제를 처리하고 있는 Bootstrap 같은 라이브러리를 사용합니다.
  - `autoprefixer`를 사용하여 벤더 프리픽스를 코드에 자동으로 추가합니다.
  - Reset CSS 또는 Normalize.css를 사용합니다.

* **기능이 제한된 브라우저의 페이지는 어떻게 처리하나요? 어떤 기술/프로세스를 사용하나요?**

  - 우아한 퇴보 - 최신 브라우저를 위한 어플리케이션을 구축하는 동시에 그것이 구형 브라우저에서도 계속 작동하도록 하는 구축방법.
  - 점진적 향상 - 기본 수준의 사용자 환경에 대한 응용 프로그램을 구축하지만 브라우저가 이를 지원할 경우 기능을 강화하는 방법.
  - [caniuse.com](https://caniuse.com/)을 사용하여 기능 지원을 확인합니다.
  - 자동 벤더 프리픽스 삽입을 위해 Autoprefixer 사용.
  - [Modernizr](https://modernizr.com/)를 사용하여 기능 감지.
  - CSS Feature 쿼리 [@support](https://developer.mozilla.org/en-US/docs/Web/CSS/@supports) 사용.

- **시각적으로 보이지 않고 스크린 리더에서만 가능하게 하는 방법에 관해 설명해주세요.**

  이러한 기술은 Accessibility(a11y)에 관련이 있습니다.

  - `visibility: hidden`. 하지만, 요소는 여전히 페이지의 흐름에 여전히 공간을 차지하게 됩니다.
  - `width: 0; height: 0`. 요소가 화면의 어떤 공간도 차지하지 않도록 합니다. 결과적으로 보이지 않게 됩니다.
  - `position: absolute; left: -99999px`. 화면 외부에 배치합니다.
  - `text-indent: -9999px`. 이것은 `block`인 요소 내의 텍스트에서만 작동합니다.
  - 메타데이터. 예를 들면, Schema.org, RDF, JSON-LD를 사용합니다.
  - WAI-ARIA. 웹 페이지의 Accessibility를 높이는 방법을 정의하는 W3C 기술 사양입니다.

  WAI-ARIA가 이상적인 해결책이라 하더라도 저는 `absolute` 위치지정 접근방법을 택할 것입니다. 대부분의 요소에 작동하며 간단한 기술이기 때문입니다.

  ###### 참고자료

  - https://www.w3.org/TR/wai-aria-1.1/
  - https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA
  - http://a11yproject.com/

* **그리드 시스템(Grid system)을 사용한 적이 있나요? 있다면 어떠한 것을 선호하나요?**

  저는는 `float` 기반 그리드 시스템을 좋아합니다. 왜냐하면, 여전히 기존 대체할만한 시스템(flex, grid) 중에서도 가장 많은 브라우저를 지원하기 때문입니다. 이것은 `Bootstrap`에서 수 년동안 사용되었으며, 효과가 있다는 것이 입증되었습니다.

- **미디어 쿼리(media queries)를 사용한 적이 있나요? 혹은 모바일에 맞는 layout과 CSS를 사용한 적이 있나요?**

  네. 한가지 예를 들면, 여러 줄 형식의 네비게이션을 특정 breakpoint를 지나면 `fixed-bottom tab` 형태로 변환하였습니다.

* **SVG를 스타일링하는데 익숙하신가요?**

  네, 객체의 속성을 지정하는 방법을 포함해 inline CSS, CSS section 삽입, 외부 CSS file처럼 shape의 색상을 정하는 여러 방법이 있습니다. 웹에서 볼 수 있는 대부분의 SVG는 inline CSS를 사용하지만, 각각 장단점이 있습니다.

  기본적인 채색은 노드에 `fill`과 `stroke` 두 속성을 설정하여 정할 수 있습니다. `fill`은 객체 안쪽 색을 설정하고, `stroke`는 객체 주위에 그려지는 선의 색을 설정합니다. 색상 이름 (`red` 등), RGB값 (`rgb(255,0,0)`), 16진수 값, RGBA 값 등 HTML에서 사용하는 것과 동일한 CSS 색상 이름 스킴을 사용할 수 있습니다. HTML에서 사용하는 것과 동일한 CSS 색상 지정 스킴을 사용할 수 있습니다.

  ```html
  <rect
    x="10"
    y="10"
    width="100"
    height="100"
    stroke="blue"
    fill="purple"
    fill-opacity="0.5"
    stroke-opacity="0.8"
  />
  ```

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Fills_and_Strokes

- **screen이 아닌 @media 속성의 예를 들어줄 수 있나요?**

  네, @media 속성은 _screen_ 을 포함하여 4가지 타입이 있습니다.

  - all - 모든 미디어 기기 장치
  - print - 프린터
  - speech - 화면을 크게 읽는 스크린리더
  - screen - 컴퓨터 스크린, 태블릿, 스마트폰 등

  `print` 미디어 타입의 사용 예제:

  ```css
  @media print {
    body {
      color: black;
    }
  }
  ```

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/CSS/@media#Syntax

* **효율적인 CSS를 작성하는데 있어서 어려움은 무엇인가요?**

  먼저, 브라우저는 선택자가 맨 오른쪽(key 선택자)부터 왼쪽으로 일치하는지 확인합니다. 브라우저는 선택자에 따라 DOM의 요소를 필터링하고 해당 부모요소가 일치하는지 식별합니다. 선택자 체인의 길이가 짧을수록 브라우저는 해당 요소가 선택자와 일치하는지 여부를 빠르게 판별할 수 있습니다. 따라서 태그 선택자와 보편적인 선택자 사용을 피해야 합니다. 이들은 많은 요소가 매치되기 때문에 부모가 일치하는지 여부를 판단하기 위해 브라우저가 많은 작업을 해야합니다.

  [BEM (Block Element Modifier)](https://bem.info/) 방법론에서는 모두 단일 클래스를 갖고, 계층구조가 필요한 곳에서는 클래스의 이름을 확장하기를 권장합니다. 따라서 선택자를 쉽고 효율적으로 재정의할 수 있습니다.

  어떤 CSS 속성이 reflow, repaint, compositing을 트리거 하는지 알아두세요. 가능하면 레이아웃(reflow 트리거)를 변경하는 스타일은 피하세요.

  ###### 참고자료

  - https://developers.google.com/web/fundamentals/performance/rendering/
  - https://csstriggers.com/

- **CSS 전처리기를 사용하면 어떤 장단점이 있나요?**

  **장점:**

  - CSS의 유지보수성이 향상됩니다.
  - 중첩 선택자를 작성하기 쉽습니다.
  - 일관된 테마를 위한 변수사용. 여러 프로젝트에 걸쳐 테마 파일을 공유할 수 있습니다.
  - 반복되는 CSS를 위한 Mixins 생성.
  - 코드를 여러 파일로 나눕니다. CSS 파일도 나눌 수 있지만, 그렇게 하기 위해서는 각 CSS 파일을 다운로드하기 위한 HTTP 요청이 필요합니다.

  **단점:**

  - 전처리기를 위한 도구가 필요합니다. 다시 컴파일하는 시간이 느릴 수도 있습니다.

* **사용했던 CSS 전처리기에 대해 좋았던 점과 싫었던 점을 설명해주세요.**

  - **좋은 점:**

    - 대부분의 장점은 위에서 언급했습니다.
    - Less는 자바스크립트로 작성되었으며, Node와 잘 작동합니다.

  - **싫은 점:**

    - 저는 C++로 작성된 LibSass 바인딩인 `node-sass`를 통해 Sass를 사용합니다. 노드 버전을 바꿀 때 자주 다시 컴파일해야 했습니다.

    - Less에서는 변수 이름의 접두어가 `@`이며, `@media`, `@import`, `@font-face` 규칙과 같은 고유 CSS 키워드와 혼동될 수 있습니다.

- **페이지에서 표준 폰트가 아닌 폰트 디자인을 사용할 때 어떤 방식으로 처리하시나요?** (웹폰트를 제외하고)

  `font-face`를 사용하고 `font-weight`가 다른 경우 `font-family`를 정의합니다.

* **CSS Selector가 어떠한 원리로 동작하는지 설명해주세요.**

  이는 위의 효율적인 CSS 작성과 관련있습니다. 브라우저는 선택자를 오른쪽(선택자)에서부터 왼쪽으로 일치시킵니다. 브라우저는 선택자에 따라 DOM의 요소를 필터링하고 부모요소를 검사하여 일치를 판정합니다. 선택자 체인의 길이가 짧을수록, 브라우저가 해당 요소가 일치하는지 여부를 더 빠르게 판단할 수 있습니다.

  예를 들어, 이 선택자 `p span`는 먼저 모든 `요소를 찾아 그 부모의 루트까지 모두 통과하여`요소를 찾습니다. 특정한 `의 경우`를 찾는 즉시 ``이 일치하는 것을 알고있으며, 이에 따라 매칭을 중지합니다.

  ###### 참고자료

  - https://stackoverflow.com/questions/5797014/why-do-browsers-match-css-selectors-from-right-to-left

- **pseudo-elements에 관해서 설명하고 어디에서 사용되는지 이야기해보세요.**

  CSS Pseudo-element는 선택자에 추가되는 키워드로, 선택한 요소의 특정 부분을 스타일링 할 수 있습니다. 마크업을 수정하지 않고(`:before`, `:after`) 텍스트 데코레이션을 위해 사용하거나(`:first-line`, `:first-letter`) 마크업에 요소를 추가할 수 있습니다.(`content: ...`와 결합)

  - `:first-line`과 `:first-letter`는 텍스트를 데코레이션하는데 사용될 수 있습니다.
  - 위의 `.clearfix`에 사용되어 `clear: both`로 영역을 차지하지 않는 요소를 추가합니다.
  - 툴팁의 삼각 화살표는 `:before`와 `:after`를 사용합니다. 삼각형이 실제로 DOM이 아닌 스타일의 일부로 간주되기 때문에 분리하는 것이 좋습니다. 추가적인 HTML 요소를 사용하지 않고 CSS 스타일만으로 삼각형을 그릴 수는 없습니다.

* **box model에 관해 설명하고 브라우저에서 어떻게 동작하는지 설명해주세요.**

  CSS 박스 모델은 문서 트리의 요소에 대해 생성되고 시각적 포매팅 모델에 따라 배치된 사각형 상자를 나타냅니다. 각 박스에는 content 영역(예: 텍스트, 이미지 등)과 `padding`, `border`, `margin` 영역을 선택적으로 사용할 수 있습니다.

  CSS 박스 모델은 다음을 계산합니다.

  - 블록 요소가 공간을 얼마나 차지하는지.
  - 테두리 또는 여백이 겹치거나 충돌하는지 여부.
  - 박스의 크기.

  박스 모델에는 다음과 같은 규칙이 있습니다.

  - 블록 요소의 크기는 `width`, `height`, `padding`, `border`, `margin`에 의해 계산됩니다.
  - `height` 가 지정되어있지 않으면, 블럭 요소는 포함하고있는 내용만큼의 높이를 가질 것이고, `padding`을 더합니다.(float가 아닌경우).
  - `width` 가 지정되지있지 않으면, float가 아닌 블록 요소는 [부모의 너비-`padding`]에 맞게 확장됩니다.
  - 요소의 `height`는 내용의 `height`에 의해 계산됩니다.
  - 요소의 `width`는 내용의 `width`에 의해 계산됩니다.
  - 기본적으로, `padding`과 `border`는 요소의 `width`와 `height`의 일부가 아닙니다.

  ###### 참고자료

  - https://www.smashingmagazine.com/2010/06/the-principles-of-cross-browser-css-coding/#understand-the-css-box-model

- **`* { box-sizing: border-box; }`은 무엇이고 사용했을때 이점은 무엇인가요?**

  - 기본적으로, 요소들에 `box-sizing: content-box`가 적용되면, 내용의 크기만 고려됩니다.
  - `box-sizing: border-box`는 요소의 `width`와 `height`가 어떻게 계산되는지를 변경하여, `border`와 `padding`도 계산에 포함됩니다.
  - 요소의 `height`는 내용의 [`height` + 수직 `padding` + 수직 `border` 폭]으로 계산됩니다.
  - 요소의 `width` 는 내용의 [`width` + 수평 `padding` + 수평 `border` 폭]으로 계산됩니다.
  - `padding`과 `border`를 박스 모델의 일부분으로 생각하면, 디자이너가 실제로 생각하는 것과 잘 들어 맞습니다.

  ###### 참고자료

  - https://www.paulirish.com/2012/box-sizing-border-box-ftw/

* **기억나는 display 속성에 대한 값들을 나열해보세요.**

  none, block, inline, inline-block, table, table-row, table-cell, list-item.

- **inline과 inline-block의 차이점은 무엇인가요?**

  좋은 비교를 위해 `block` 과도 비교해 볼 것입니다.

  ![img](https://media.vlpt.us/post-images/chris/00ccfe60-5f8e-11e9-b975-e5b35539d0db/image.png)

* **요소를 배치하는 방법(relative, fixed, absolute, static) 간의 차이는 무엇인가요?**

  위치가 정해진 요소는 계산된 `position` 속성이 `relative`, `absolute`, `fixed`, `sticky` 중 하나인 요소입니다.

  - `static` - 기본 위치. 요소가 평소와 같이 페이지에 위치합니다. `top`, `right`, `bottom`, `left`, `z-index` 속성은 적용되지 않습니다.
  - `relative` - 요소의 위치가 레이아웃을 변경하지 않고, 자체에 상대적으로 조정됩니다. (따라서 배치되지 않은 요소의 간격을 남겨 둡니다.)
  - `absolute` - 요소가 페이지의 평소 위치에서 제거되고, 가장 가까운 `relative` 부모 블록이 있는 경우 지정된 위치에 배치됩니다. 그렇지 않으면 최상위 블록에 의존됩니다. absolute로 배치된 박스는 margin을 가질 수 있으며 다른 margin과 충돌하지 않습니다. 이 요소는 다른 요소의 위치에 영향을 주지 않습니다.
  - `fixed` - 요소는 페이지의 평소 위치에서 제거되고 뷰포트를 기준으로 지정된 위치에 배치되며 스크롤 할 때 이동하지 않습니다.
  - `sticky` - sticky는 `relative`와 `fixed`의 하이브리드입니다. 요소는 지정된 임계값을 넘을 때까지 `relative` 위치로 처리되며, 특정 지점에서 `fixed` 위치로 처리됩니다.

  ###### 참고자료

  - https://developer.mozilla.org/en/docs/Web/CSS/position

- **CSS에서 'C’는 Cascading을 의미합니다. Cascading에 관해서 설명해주세요. 또 cascading system의 장점은 무엇인가요?**

  Cascading은 계단모양의 폭포를 의미하며 CSS에서 스타일 시트의 **우선순위**를 지정하는 방식이 폭포수와 닮아 붙여진 의미 입니다.
  cascading system을 사용하였을 때의 장점은 HTML Element마다 일일이 스타일을 지정하지 않아도 되므로 렌더링 속도와 코드의 양을 줄여 성능 향상에 기여할 수 있습니다.

* **CSS framework를 사용해본 적이 있으신가요? 실무에서 사용해보았다면 어떤 이점이 있었나요?**

  부트스트랩, Angular Material을 사용해보았습니다.
  실무에서 사용했을때 우선 직접적으로 모든 스타일링을 하지 않고,
  프레임워크에서 제공하는 컴포넌트들을 사용하기 때문에 시간을 절약할 수 있습니다.
  또한 사용자에게 일관된 디자인을 제공할 수 있습니다.

- **새로운 CSS Flexbox 혹은 Grid 스펙을 사용해 보신 적 있나요?**

  Flexbox는 주로 1차원 레이아웃을 대상으로 하며 Grid는 2차원 레이아웃을 대상으로 합니다.

  Flexbox는 CSS에서 컨테이너 안에 있는 요소의 수직 가운데정렬, sticky footer 등과 같은 많은 일반적인 문제들을 해결합니다. Bootstrap과 Bulma는 Flexbox를 기반으로 하고, 이는 아마도 요즘 레이아웃을 만드는 데 권장되는 방법일 것입니다. 이전에 Flexbox를 사용해 보았지만, `flex-grow`를 사용할 때 일부 브라우저에서 비호환성 문제(Safari)가 발생했습니다. 그래서 백분율로 나타낸 폭을 계산하기 위해 `inline-blocks`과 수학을 사용한 코드로 다시 써야했는데, 이는 좋은 경험은 아니었습니다.

  Grid는 그리드 기반의 레이아웃을 생성하기 위한 가장 직관적인 접근법이지만(더 좋을 것입니다!), 현재 브라우저 지원은 넓지 않습니다.

  ###### 참고자료

  - https://philipwalton.github.io/solved-by-flexbox/

* **반응형 웹사이트를 코딩하는 것과 모바일 우선 전략을 사용하는 것 사이의 차이점을 설명하세요.**

  이 두가지 접근법은 배타적이지 않습니다.

  반응형 웹사이트를 만드는 것은 일부 요소가 미디어 쿼리를 통해 장치의 화면 크기(일반적으로 뷰포트 너비)에 따라 크기나 다른 기능을 조정하도록 반응함을 의미합니다. (예: 작은 디바이스에서 글꼴 크기를 줄임)

  ```css
  @media (min-width: 601px) {
    .my-class {
      font-size: 24px;
    }
  }
  @media (max-width: 600px) {
    .my-class {
      font-size: 12px;
    }
  }
  ```

  모바일 우선 전략 또한 반응적이지만, 모바일 장치에 대한 모든 스타일을 정의해야하며 나중에 다른 장치에 대한 특정 규칙을 추가해야합니다. 이전 예를 따르면 다음과 같습니다.

  ```css
  .my-class {
    font-size: 12px;
  }

  @media (min-width: 600px) {
    .my-class {
      font-size: 24px;
    }
  }
  ```

  모바일 우선 전략은 2가지 주요 장점을 가지고 있습니다.

  - 모바일 장치에서 적용되는 모든 규칙이 미디어 쿼리에 대해 유효성 검사를 받을 필요가 없으므로 모바일 장치에서 더 뛰어난 성능을 발휘합니다.
  - 반응형 CSS 규칙과 관련하여 보다 명확한 코드를 작성해야합니다.

- **반응형(Responsive) 디자인은 적응형(Adaptive) 디자인과 어떤 차이점이 있나요?**

  반응형과 적응형 디자인은 모두 서로 다른 뷰포트 사이즈, 해상도, 사용 컨텍스트, 제어 메커니즘 등을 조정하여 다양한 장치에서 사용자 경험을 최적화하려고 시도합니다.

  반응형 디자인은 유연성 원칙에 따라 작동합니다. 즉, 어떤 장치에서나 보기 좋은 단일 변하기 쉬운 웹 사이트입니다. 반응형 웹 사이트는 미디어 쿼리, 유연한 그리드 및 반응 형 이미지를 사용하여 다양한 요인에 따라 유연하고 변화하는 사용자 경험을 제공합니다. 마치 하나의 공이 여러개의 서로 다른 링을 통과하기 위해 커지거나 줄어드는 것과 유사합니다.

  적응형 디자인는 점진적 향상의 현대적 정의에 더 가깝습니다. 하나의 유연한 디자인 대신에, 적응형 설계는 장치 및 기타 기능을 감지 한 다음 사전 정의 된 뷰포트 크기 및 기타 특성 세트를 기반으로 적절한 기능 및 레이아웃을 제공합니다. 하나의 공이 여러개의 서로 다른 링을 통과하는 대신, 링의 크기에 따라 여러개의 공을 사용하는 것과 유사합니다.

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Archive/Apps/Design/UI_layout_basics/Responsive_design_versus_adaptive_design
  - http://mediumwell.com/responsive-adaptive-mobile/
  - https://css-tricks.com/the-difference-between-responsive-and-adaptive-design/

* **레티나 그래픽 환경에서 작업해 보신 적이 있나요? 하셨다면 어떤 기술을 사용하셨나요?**

  _레티나_ 는 픽셀 비율이 1보다 큰 고해상도 화면을 나타내는 마케팅 용어 일뿐입니다. 중요하게 알아야할 것은 픽셀 비율을 사용하면 이러한 디스플레이가 동일한 크기의 요소를 표시하기 위해 더 저해상도의 화면으로 표현한다는 것입니다.
  요즘에는 모든 모바일 디바이스를 _레티나_ 디스플레이로 간주합니다.

  브라우저는 기본적으로 이미지들을 제외하고 디바이스의 해상도에 따라 DOM 요소를 렌더링합니다.

  레티나 디스플레이를 최상으로 만드는 선명하고보기 좋은 그래픽을 얻으려면 가능한한 고해상도 이미지를 사용해야합니다. 하지만 항상 가장 높은 해상도의 이미지를 사용하면 더 많은 바이트가 전송되어야 하기 때문에 성능에 영향을 미칩니다.

  이 문제를 극복하기 위해, HTML5에 스펙인 반응형 이미지를 사용할 수 있습니다. 이는 동일한 이미지의 다른 해상도 파일을 브라우저에 제공하고 html 속성 `srcset`과 `sizes`를 사용하여 어떤 이미지가 가장 적합한지 결정하도록합니다.

  ```html
  <div responsive-background-image>
    <img
      src="/images/test-1600.jpg"
      sizes="
        (min-width: 768px) 50vw,
        (min-width: 1024px) 66vw,
        100vw"
      srcset="
        /images/test-400.jpg   400w,
        /images/test-800.jpg   800w,
        /images/test-1200.jpg 1200w
      "
    />
  </div>
  ```

  HTML5의 `srcset`를 지원하지 않는 브라우저(예: IE11)는 이를 무시하고 대신 `src`로 사용한다는 것을 알고있어야 합니다. IE11를 정말 지원해야하고 성능상의 이유로 이 기능을 제공해야하는 경우 자바스크립트 폴리필을 사용할 수 있습니다. 예: Picturefill(참고자료 링크)

  아이콘의 경우, SVG나 아이콘폰트를 사용하면 해상도에 관계없이 매우 선명하게 렌더링되므로 가능하면 이를 사용합니다.

  ###### 참고자료

  - https://css-tricks.com/responsive-images-youre-just-changing-resolutions-use-srcset/
  - http://scottjehl.github.io/picturefill/
  - https://aclaes.com/responsive-background-images-with-srcset-and-sizes/

- **absolute 포지셔닝 대신 translate()를 사용하는 이유가 무엇인가요? 또는 그 반대의 경우에 대해서는 어떻게 생각하시나요?, 그 이유는 무엇인가요?**

  `translate()`은 CSS `transform`의 값입니다. `transform`이나 `opacity`를 변경해도 브라우저의 reflow나 repaint가 다시 발생하지 않고 컴포지션만 실행되는 반면, 절대 위치를 변경하면 `reflow`가 발생합니다. `transform`을 사용하면 브라우저에서 이 요소를 위한 GPU 레이어가 생성되지만, 절대 위치 속성을 변경하는 것은 CPU를 사용합니다. 그러므로 `translate()`가 더 효율적이며, 매끄러운 애니메이션을 위한 페인트 시간이 짧아집니다.

  `translate()`을 사용할 때는 절대 위치를 변경할 때와 달리 원래 위치(일종의 `position: relative`)를 그대로 사용합니다.

  ###### 참고자료

  - https://www.paulirish.com/2012/why-moving-elements-with-translate-is-better-than-posabs-topleft/

### References

- https://ksw1652.github.io/2018/08/14/front-end-interview-css-question/
- https://velog.io/@chris/front-end-interview-handbook-css-3
- [https://quizlet.com/kr/480880508/html-css-%EC%A7%88%EB%AC%B8-flash-cards/](https://quizlet.com/kr/480880508/html-css-질문-flash-cards/)

---

## JS 관련 질문:

- **event delegation(이벤트 위임)에 관해 설명해주세요.**

  이벤트 위임은 이벤트 리스너를 하위 요소에 추가하는 대신 상위 요소에 추가하는 기법입니다. 리스너는 DOM의 event bubbling으로 인해 하위 요소에서 이벤트가 발생될 때마다 실행됩니다. 이 기술의 이점은 다음과 같습니다.

  - 각 하위 항목에 이벤트 핸들러를 연결하지 않고, 상위 요소에 하나의 단일 핸들러만 필요하기 때문에 메모리 사용 공간이 줄어듭니다.
  - 제거된 요소에서 핸들러를 해제하고 새 요소에 대해 이벤트를 바인딩할 필요가 없습니다.

  ###### 참고자료

  - https://davidwalsh.name/event-delegate
  - https://stackoverflow.com/questions/1687296/what-is-dom-event-delegation

* **`this`는 JavaScript에서 어떻게 작동하는지 설명해주세요.**

  `this`는 간단하게 설명하기 어렵습니다. JavaScript에서 가장 혼란스러운 개념 중 하나입니다. 대략 설명하면 `this`의 값은 함수가 호출되는 방식에 따라 달라집니다. 온라인에 많은 설명을 읽었는데, [Arnav Aggrawal](https://medium.com/@arnav_aggarwal)의 설명이 가장 명확했습니다.
  다음 규칙과 같습니다.

  1. 함수를 호출할 때 `new` 키워드를 사용하는 경우, 함수 내부에 있는 `this`는 완전히 새로운 객체입니다.
  2. `apply`, `call`, `bind`가 함수의 호출/생성에 사용되는 경우, 함수 내의 `this`는 인수로 전달된 객체입니다.
  3. `obj.method()`와 같이 함수를 메서드로 호출하는 경우, `this`는 함수가 프로퍼티인 객체입니다.
  4. 함수가 자유함수로 호출되는 경우, 즉, 위의 조건 없이 호출되는 경우 `this`는 전역 객체입니다. 브라우저에서는 `window` 객체입니다. 엄격 모드(`'use strict'`) 일 경우, `this`는 전역 객체 대신 `undefined`가 됩니다.
  5. 위의 규칙 중 다수가 적용되면 더 상위 규칙이 승리하고 `this`값을 설정합니다.
  6. 함수가 ES2015 화살표 함수인 경우 위의 모든 규칙을 무시하고 생성된 시점에서 주변 스코프의 `this`값을 받습니다.

  상세한 설명은 [Medium의 글](https://codeburst.io/the-simple-rules-to-this-in-javascript-35d97f31bde3)을 참조하세요.

  ###### References

  - https://codeburst.io/the-simple-rules-to-this-in-javascript-35d97f31bde3
  - https://stackoverflow.com/a/3127440/1751946

- **prototype 기반 상속은 어떻게 하는지 설명해주세요.**

  이는 매우 일반적인 JavaScript 인터뷰 질문입니다. 모든 JavaScript 객체는 다른 객체에 대한 참조인 `prototype` 프로퍼티를 가지고 있습니다. 객체의 프로퍼티에 접근할 때, 해당 객체에 해당 프로퍼티가 없으면 JavaScript 엔진은 객체의 `prototype`과 `prototype`의 `prototype`등을 보고 프로퍼티 정의가 있을 때까지 찾고, 만약 객체의 프로퍼티에 접근할 때 해당 객체에 해당 프로퍼티가 없으면 프로토타입 체인 중 하나에 있거나 프로토타입 체인의 끝에 도달할 때까지 찾습니다. 이 동작은 고전적인 상속을 흉내내지만, 실제로 [상속보다 위임](https://davidwalsh.name/javascript-objects)에 더 가깝습니다.

  ###### 참고자료

  - https://www.quora.com/What-is-prototypal-inheritance/answer/Kyle-Simpson
  - https://davidwalsh.name/javascript-objects

* **AMD와 CommonJS는 무엇이고, 이것들에 대해 어떻게 생각하시나요?**

  두 가지 모두 ES2015가 등장하기 전까지 JavaScript에 기본적으로 존재하지 않는 모듈 시스템을 구현하는 방법입니다. CommonJS는 동기식인 반면 AMD(Asynchronous Module Definition - 비동기식 모듈 정의)는 분명히 비동기식입니다. CommonJS는 서버사이드 개발을 염두에 두고 설계되었으며, AMD는 모듈의 비동기 로딩을 지원하므로 브라우저용으로 더 많이 사용됩니다.

  AMD은 구문이 매우 장황하고, CommonJS은 다른 언어처럼 import 문을 작성하는 스타일에 더 가깝습니다. 대부분의 경우 AMD를 필요로 하지 않습니다. 모든 JavaScript를 연결된 하나의 번들 파일로 제공하면 비동기 로딩 속성의 이점을 누릴 수 없기 때문입니다. 또한 CommonJS 구문은 모듈 작성의 노드 스타일에 가깝고 클라이언트 사이드와 서버사이드 JavaScript 개발 사이를 전환할 때 문맥 전환 오버 헤드가 적습니다.

  ES2015 모듈이 동기식 및 비동기식 로딩을 모두 지원하는 것이 반가운 것은 마침내 하나의 접근 방식만 고수할 수 있다는 점입니다. 브라우저와 노드에서 완전히 작동되지는 않지만, 언제나 트랜스파일러를 사용하여 코드를 변환할 수 있습니다.

  ###### 참고자료

  - https://auth0.com/blog/javascript-module-systems-showdown/
  - https://stackoverflow.com/questions/16521471/relation-between-commonjs-amd-and-requirejs

- **다음 코드가 즉시 호출 함수 표현식(IIFE)로 동작하지 않는 이유에 관해서 설명해보세요:**

  ```javascript
  function foo(){ }();
  ```

  - **IIFE로 만들기 위해서는 어떻게 해야 하나요?**

  IIFE는 즉시 함수 호출 표현식(Immediately Invoked Function Expressions)을 의미합니다. JavaScript parser는 `function foo(){ }();`을 `function foo(){ }`와 `();`로 읽습니다. 전자는 **함수 선언**이며 후자(한 쌍의 중괄호)는 함수를 호출하려고 시도했지만, 이름이 지정되지 않았기 때문에 `Uncaught SyntaxError : Unexpected token )`을 발생시킵니다.

  괄호를 추가하여 고치는 두 가지 방법이 있습니다: `(function foo(){ })()` 그리고 `(function foo(){ }())`. `function`으로 시작하는 문은 **함수 선언**으로 간주됩니다. 이 함수를 `()`로 묶으면 **함수 식**이 되고, 이렇게하면 다음 `()`로 함수를 실행할 수 있습니다. 이러한 함수는 전역 범위에 노출되지 않으며, 본문 내에서 이 함수 자체를 참조할 필요가 없는 경우에는 해당 함수의 이름을 생략할 수도 있습니다.

  `void function foo(){ }();`처럼 `void` 연산자를 사용할 수도 있습니다. 불행히도, 이러한 접근방식에는 한 가지 문제가 있습니다. 주어진 표현식의 평가는 항상 `undefined`이므로, IIFE 함수가 무언가를 반환하면, 사용할 수 없습니다. 예:

  ```js
  // Don't add JS syntax to this code block to prevent Prettier from formatting it.
  const foo = void (function bar() {
    return "foo";
  })();

  console.log(foo); // undefined
  ```

  ###### 참고자료

  - http://lucybain.com/blog/2014/immediately-invoked-function-expression/
  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/void

* **`null` 과 `undefined` , `undeclared` 의 차이점은 무엇인가요?**

  - **두개를 구분하기 위해서는 어떻게 하면 될까요?**

  **Undeclared** 변수는 이전에 `var`, `let`, `const`를 사용하여 생성되지 않은 식별자에 값을 할당할 때 생성됩니다. `Undeclared` 변수는 현재 범위 외부에 전역으로 정의됩니다. strict 모드에서는 `Undeclared` 변수에 할당하려고 할 때, `ReferenceError`가 발생합니다. `Undeclared` 변수는 전역 변수처럼 좋지 않습니다. 이것들은 모두 사용을 피하세요! 이를 검사하려면, 사용할 때 `try`/`catch` 블록에 감싸세요.

  ```js
  function foo() {
    x = 1; // strict 모드에서 ReferenceError를 발생시킵니다.
  }

  foo();
  console.log(x); // 1
  ```

  `undefined` 변수는 선언되었지만, 값이 할당되지 않은 변수입니다. 이는 `undefined` 타입입니다. 함수가 실행 결과에 따라 아무값도 반환하지 않으면, 변수에 할당되며, 그 변수가 `undefined` 값을 갖습니다. 이를 검사하기 위해, 엄격한 (`===`) 연산자 또는 `typeof`에 `undefined` 문자열을 사용하여 비교하세요. 확인을 위해 추상 평등 연산자(`==`)를 사용해서는 안되며, 이는 값이 `null`이면 `true`를 반환합니다.

  ```js
  var foo;
  console.log(foo); // undefined
  console.log(foo === undefined); // true
  console.log(typeof foo === "undefined"); // true

  console.log(foo == null); // true. 옳지않습니다. 이렇게 사용하지 마세요.

  function bar() {}
  var baz = bar();
  console.log(baz); // undefined
  ```

  `null`인 변수는 `null` 값이 명시적으로 할당된 것입니다. 그것은 값을 나타내지 않으며, 명시적으로 할당됐다는 점에서 `undefined`와 다릅니다. `null`을 체크하기 위해서 단순히 완전 항등 연산자(`===`)를 사용하여 비교하면 됩니다. 위와 같이, 추상 평등 연산자 (`==`)를 사용해서는 안되며, 값이 `undefined`이면 `true`를 반환합니다.

  ```js
  var foo = null;
  console.log(foo === null); // true

  console.log(foo == undefined); // true. 옳지않습니다. 이렇게 사용하지 마세요.
  ```

  개인적 습관으로, 저는 변수를 선언하지 않거나(undeclared) 할당하지 않은 상태(unassigned)로 두지 않습니다. 아직 사용하지 않으려는 경우, 선언한 후에 명시적으로 `null`을 할당할 것입니다. 작업시 linter를 사용하면, 일반적으로 Undeclared 변수를 참조하지는 않는지 확인할 수 있습니다.

  ###### 참고자료

  - https://stackoverflow.com/questions/15985875/effect-of-declared-and-undeclared-variables
  - https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/undefined

- **클로져(Closure)는 무엇이며, 어떻게/왜 사용하는지 설명해주세요.**

  - **클로져를 만들 때 선호하는 패턴은 무엇인가요? argyle (IIFEs에만 적용할 수 있다)**

  클로저는 함수와 그 함수가 선언된 렉시컬 환경의 조합입니다. "렉시컬"은 렉시컬 범위 지정이 변수가 사용 가능한 위치를 결정하기 위해 소스 코드 내에서 변수가 선언된 위치를 사용한다는 사실을 나타냅니다. 클로저는 외부 함수가 반환된 후에도 외부 함수의 변수 범위 체인에 접근할 수 있는 함수입니다.

  **왜 클로저를 사용합니까?**

  - 클로저로 데이터 프라이버시 / private method를 모방. 일반적으로 [모듈 패턴](https://addyosmani.com/resources/essentialjsdesignpatterns/book/#modulepatternjavascript)에 사용됩니다.
  - [부분 적용 또는 currying](https://medium.com/javascript-scene/curry-or-partial-application-8150044c78b8#.l4b6l1i3x).

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures
  - https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36

* **.forEach 루프와 .map() 루프 사이의 주요 차이점을 설명할 수 있나요? 왜 둘 중 하나를 선택할 것인가요?**

  이 두 함수의 차이점을 이해하기 위해 각 함수가 무엇을 하는지 살펴보겠습니다.

  **`forEach`**

  - 배열의 요소를 반복합니다.
  - 각 요소에 대해 콜백을 실행합니다.
  - 값을 반환하지 않습니다.

  ```js
  const a = [1, 2, 3];
  const doubled = a.forEach((num, index) => {
    // num나 index로 무언가 합니다.
  });

  // doubled = undefined
  ```

  **`map`**

  - 배열의 요소를 반복합니다.
  - 각 요소에서 함수를 호출하여 결과로 새 배열을 작성하여 각 요소를 새 요소에 매핑합니다.

  ```js
  const a = [1, 2, 3];
  const doubled = a.map((num) => {
    return num * 2;
  });

  // doubled = [2, 4, 6]
  ```

  `.forEach`와 `.map()`의 가장 큰 차이점은 `.map()`이 새로운 배열을 반환한다는 것입니다. 결과가 필요하지만 원본 배열을 변경하고 싶지 않으면, `.map()`이 확실한 선택입니다. 단순히 배열을 반복할 필요가 있다면, `forEach`가 좋은 선택입니다.

  ###### 참고자료

  - https://codeburst.io/javascript-map-vs-foreach-f38111822c0f

- **익명함수(anonymous functions)는 주로 어떤 상황에서 사용하나요?**

  익명함수는 IIFE로 사용되어 지역 범위 내에서 일부 코드를 캡슐화하므로 선언된 변수가 전역 범위로 누출되지 않습니다.

  ```js
  (function () {
    // 코드
  })();
  ```

  한 번 사용되고 다른 곳에서는 사용할 필요가 없는 콜백으로 사용됩니다. 함수 본체를 찾기 위해 다른 곳을 찾아볼 필요 없이 코드를 호출하는 코드 바로 안에 핸들러가 정의되어 있으면 코드가 보다 독립적이고 읽기 쉽게 보일 것입니다.

  ```js
  setTimeout(function () {
    console.log("Hello world!");
  }, 1000);
  ```

  함수형 프로그래밍 또는 Lodash에 대한 인수(콜백과 유사)로 사용.

  ```js
  const arr = [1, 2, 3];
  const double = arr.map(function (el) {
    return el * 2;
  });
  console.log(double); // [2, 4, 6]
  ```

  ###### 참고자료

  - https://www.quora.com/What-is-a-typical-usecase-for-anonymous-functions
  - https://stackoverflow.com/questions/10273185/what-are-the-benefits-to-using-anonymous-functions-instead-of-named-functions-fo

* **당신의 코드를 어떻게 구성하는지? (모듈 패턴, 전통적 상속)**

  과거에는 Backbone 모델을 만들고 그 모델에 메소드를 연결하는 등 OOP 접근 방식을 장려하는 모델에 Backbone 을 사용했습니다.

  모듈 패턴은 여전히 훌륭하지만, 요즘에는 React/Redux 기반의 Flux 아키텍처를 사용합니다. 이 아키텍처는 단방향 프로그래밍 방식을 권장합니다. 저는 평범한 객체를 사용하여 응용 프로그램의 모델을 표현하고 이러한 객체를 조작하는 유틸리티 순수 함수를 작성합니다. 상태는 다른 Redux 응용 프로그램에서와 마찬가지로 action 및 reducer를 사용하여 조작됩니다.

  가능한 경우 고전적인 상속을 사용하지 않습니다. 저는 [이 규칙들](https://medium.com/@dan_abramov/how-to-use-classes-and-sleep-at-night-9af8de78ccb4)을 유지합니다.

- **호스트 객체(Host Objects)와 네이티브 객체(Native Objects)의 차이점은 무엇인가요?**

  내장 객체는 ECMAScript 사양에 정의된 JavaScript 언어의 일부인 객체입니다. (예: `String`, `Math`, `RegExp`, `Object`, `Function` 등)

  호스트 객체는 `window`, `XMLHTTPRequest` 등과 같이 런타임 환경 (브라우저 or 노드)에 의해 제공됩니다.

  ###### 참고자료

  - https://stackoverflow.com/questions/7614317/what-is-the-difference-between-native-objects-and-host-objects

* **다음 코드의 차이점은 무엇인가요?**

  ```js
  function Person(){} var person = Person() var person = new Person()
  ```

  이 질문은 굉장해 애매합니다. 질문의 의도에 대한 저의 최선의 추측은 JavaScript의 생성자에 대해 묻는 것입니다. 엄밀히 말하면, `function Person(){}`은 정상적인 함수 선언일 뿐입니다. 이 컨벤션은 함수생성자로 사용하기 위해 함수이름에 PascalCase를 사용합니다.

  `var person = Person()`은 생성자가 아니며 `Person`을 함수로 호출합니다. 함수를 생성자로 사용하려는 경우에 이렇게 호출하는 것은 일반적인 실수입니다. 일반적으로 생성자는 아무것도 반환하지 않으므로 일반 함수처럼 생성자를 호출하면 `undefined`가 반환되고 지정된 변수에 할당됩니다.

  `var person = new Person()`은 `Person.prototype`을 상속받은 `new` 연산자를 사용하여 `Person` 객체의 인스턴스를 생성합니다. 또 다른 방법은 `Object.create`를 사용하는 것입니다: `Object.create(Person.prototype)`.

  ```js
  function Person(name) {
    this.name = name;
  }

  var person = Person("John");
  console.log(person); // undefined
  console.log(person.name); // Uncaught TypeError: Cannot read property 'name' of undefined

  var person = new Person("John");
  console.log(person); // Person { name: "John" }
  console.log(person.name); // "john"
  ```

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/new

- **`.call`과 `.apply`의 차이점은 무엇인가요?**

  `.call`과 `.apply`는 모두 함수를 호출하는데 사용되며, 첫 번째 매개변수는 함수 내에서 `this`의 값으로 사용됩니다. 그러나 `.call`은 쉼표로 구분된 인수를 두 번째 인수로 취하고 `.apply`는 인수의 배열을 두 번째 인수로 취합니다. `call`은 `C`: `Comma` 로 구분되며, `apply`는 인수 배열인 `A`: `arguments` 라고 기억하면 쉽습니다.

  ```js
  function add(a, b) {
    return a + b;
  }

  console.log(add.call(null, 1, 2)); // 3
  console.log(add.apply(null, [1, 2])); // 3
  ```

* **`Function.prototype.bind`을 설명하세요.**

  [MDN](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_objects/Function/bind)에서 인용:

  > `bind()` 메소드는 호출될 때, this 키워드가 주어진 인자 값으로 설정되고, 새로운 함수가 호출될 때, 앞쪽의 매개변수도 자신의 인자를 사용해 미리 순서대로 채워놓은 새로운 함수를 반환합니다.

  저의 경험상, 다른 함수로 전달하고자 하는 클래스의 메소드에서 `this`의 값을 바인딩할 때 가장 유용합니다. 이는 React 컴포넌트에서 자주 사용됩니다.

  ###### 참고자료

  - https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_objects/Function/bind

- **`document.write()`는 언제 사용하나요?**

  `document.write()`는 `document.open()`에 의해 열린 문서 스트림에 텍스트 문자열을 씁니다. 페이지가 로드된 후에 `document.write()`가 실행되면 `document.open`을 호출하여 문서 전체를 지우고 (`와`를 지웁니다!). 문자열로 주어진 매개 변수 값으로 대체합니다. 그러므로 일반적으로 위험하고 오용되기 쉽습니다.

  `document.write()`가 코드분석이나 [JavaScript가 활성화된 경우에만 작동하는 스타일을 포함하고 싶을 때](https://www.quirksmode.org/blog/archives/2005/06/three_javascrip_1.html) 사용되는 경우를 설명하는 온라인 답변이 몇 가지 있습니다. 심지어 HTML5 보일러 플레이트에서 [스크립트를 병렬로 로드하고 실행 순서를 보존](https://github.com/paulirish/html5-boilerplate/wiki/Script-Loading-Techniques#documentwrite-script-tag)할 때도 사용됩니다! 그러나, 저는 그 이유가 시대에 뒤떨어진 것으로 생각하고 있으며, 현재는 `document.write()`를 사용하지 않고도 할 수 있습니다. 이것이 틀렸다면 고쳐주세요.

  ###### 참고자료

  - https://www.quirksmode.org/blog/archives/2005/06/three_javascrip_1.html
  - https://github.com/h5bp/html5-boilerplate/wiki/Script-Loading-Techniques#documentwrite-script-tag

* **Feature detection, Feature inference, UA String의 차이점은 무엇인가요?**

  **Feature Detection**

  Feature Detection은 브라우저가 특정 코드 블록을 지원하는지에 따라 다른 코드를 실행하도록 하여, 일부 브라우저에서 항상 오류 대신 무언가 작동하도록 합니다. 예:

  ```js
  if ("geolocation" in navigator) {
    // navigator.geolocation를 사용할 수 있습니다
  } else {
    // 부족한 기능 핸들링
  }
  ```

  [Modernizr](https://modernizr.com/)는 Feature detection을 처리 할 수 있는 훌륭한 라이브러리입니다.

  **Feature Inference**

  Feature inference는 Feature detection과 마찬가지로 기능을 확인하지만 다른 함수도 존재한다고 가정하고 사용합니다. 예:

  ```js
  if (document.getElementsByTagName) {
    element = document.getElementById(id);
  }
  ```

  이것은 권장하지 않습니다. Feature detection이 더 확실합니다.

  **UA String**

  네트워크 프로토콜 피어가 요청하는 소프트웨어 유저 에이전트의 응용 프로그램 유형, 운영 체제, 소프트웨어 공급 업체 또는 소프트웨어 버전을 식별할 수 있도록 해주는 browser-reported String입니다. `navigator.userAgent` 를 통해 접근 할 수 있습니다. 하지만 문자열은 구문 분석하기 까다로우며 스푸핑될 수 있습니다. 예를 들어, Chrome은 Chrome과 Safari로 모두 보고됩니다. Safari를 감지하기 위해서는 Safari 문자열이 있는지와 Chrome 문자열이 없는지 확인해야 합니다. 이 방법은 사용하지 마세요.

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Cross_browser_testing/Feature_detection
  - https://stackoverflow.com/questions/20104930/whats-the-difference-between-feature-detection-feature-inference-and-using-th
  - https://developer.mozilla.org/en-US/docs/Web/HTTP/Browser_detection_using_the_user_agent

- **AJAX에 관해 가능한 한 자세히 설명하세요.**

  Ajax(asynchronous JavaScript and XML)는 비동기 웹 응용 프로그램을 만들기 위해 클라이언트 측에서 사용되는 웹 개발 기술의 집합입니다. Ajax를 사용하면 웹 애플리케이션은 기존 페이지의 화면 및 동작을 방해하지 않으면서 백그라운드에서 비동기적으로 서버로 데이터를 보내고 서버에서 데이터를 받아올 수 있습니다. Ajax는 프리젠테이션 레이어에서 데이터 교환 레이어를 분리함으로써, 웹페이지 및 확장 웹 애플리케이션이 전체 페이지를 다시 로드 할 필요 없이 동적으로 컨텐츠를 변경할 수 있도록 합니다. 실제로 최근에는 일반적으로 네이티브 JavaScript의 장점 때문에 XML대신 JSON을 사용합니다.

  `XMLHttpRequest` API는 비동기 통신에 자주 사용되며, 최근에는 `fetch` API가 자주 사용됩니다.

  ###### 참고자료

  - https://en.wikipedia.org/wiki/Ajax_(programming)
  - https://developer.mozilla.org/en-US/docs/AJAX

* **AJAX를 사용했을 때의 장단점에 대해 설명해주세요.**

  **장점**

  - 상호작용성이 좋아집니다. 서버의 새로운 컨텐츠를 전체 페이지를 다시로드할 필요 없이 동적으로 변경할 수 있습니다.
  - 스크립트나 스타일 시트는 한 번만 요청하면 되므로 서버에 대한 연결을 줄여줍니다.
  - 상태를 페이지에서 관리 할 수 있습니다. 메인 컨테이너 페이지가 다시 로드되지 않기 때문에 JavaScript의 변수와 DOM의 상태가 유지됩니다.
  - 기본적으로 SPA의 대부분의 장점과 같습니다.

  **단점**

  - 동적 웹 페이지는 북마크하기 어렵습니다.
  - 브라우저에서 JavaScript가 비활성화된 경우 작동하지 않습니다.
  - 일부 웹 크롤러는 JavaScript를 실행하지 않으며 JavaScript에 의해 로드된 콘텐츠를 볼 수 없습니다.
  - SPA의 대부분의 단점과 같습니다.

- **JSON이 어떻게 동작 되는지 설명하세요. (그리고 AJAX와 어떻게 다른지 설명하세요.)**

  JSONP(JSON with Padding)는 현재 페이지에서 cross-origin 도메인으로의 Ajax 요청이 허용되지 않기 때문에 웹 브라우저에서 cross-domain 정책을 우회하는 데 일반적으로 사용되는 방법입니다.

  JSONP는 ``태그를 통해 cross-origin 도메인에 요청하고 보통 `callback`쿼리 매개 변수(예: `https://example.com?callback=printData`)로 요청합니다. 그러면 서버는 `printData`라는 함수 안에 데이터를 래핑하여 클라이언트로 반환합니다.

  ```html
  <!-- https://mydomain.com -->
  <script>
    function printData(data) {
      console.log(`My name is ${data.name}!`);
    }
  </script>

  <script src="https://example.com?callback=printData"></script>
  // https://example.com?callback=printData 에서 로드된 파일 printData({ name:
  'Yang Shun' })
  ```

  클라이언트는 전역 범위에 있는 `printData` 함수를 가져야만 하고, cross-origin domain으로부터의 응답이 수신될 때 함수가 클라이언트에 의해 실행됩니다.

  JSONP는 안전하지 않을 수 있으며, 보안 관련 이슈가 있습니다. JSONP는 실제 JavaScript고, JavaScript가 할 수 있는 모든 작업을 수행할 수 있으므로 JSONP 데이터 공급자를 신뢰해야만 합니다.

  요즘에는 [CORS](http://en.wikipedia.org/wiki/Cross-origin_resource_sharing)가 권장되는 접근 방식이며 JSONP는 해킹으로 간주됩니다.

  ###### 참고자료

  - https://stackoverflow.com/a/2067584/1751946

* **기존에 JavaScript 템플릿을 사용한 적이 있나요? 만약에 있다면, 어떠한 방식으로 사용했는지 말씀해주세요.**

  네. Handlebars, Underscore, Lodash, AngularJS, JSX. 저는 AngularJS에서의 템플릿을 좋아하지 않았습니다. 지시자에서 문자열을 많이 사용하게 되며 오타가 감지되지 않기 때문입니다. JSX는 JavaScript에 가깝고 배워야 하는 새로운 문법이 거의 없기 때문에 더 좋아합니다. 요즘에는, Third-party 라이브러리에 의존하지 않고 템플릿을 만드는 빠른 방법으로 ES2015 템플릿 문자열 리터럴을 사용할 수도 있습니다.

  ```js
  const template = `<div>My name is: ${name}</div>`;
  ```

  그러나 템플릿 라이브러리와 달리 컨텐츠가 이스케이프되지 않으므로 위의 접근 방식에서 잠재적 XSS를 알고 있어야 합니다.

- **"호이스팅(Hoisting)"에 대해서 설명하세요.**

  호이스팅은 코드에서 변수 선언의 동작을 설명하는데 사용되는 용어입니다. `var` 키워드로 선언되거나 초기화된 변수는 현재 스코프의 최상위까지 `옮겨`집니다. 이것을 호이스팅이라고 부릅니다. 그러나 선언문만 `호이스팅`되며 할당(있는 경우)은 그대로 있게 됩니다.

  사실 선언은 실제로 이동되지 않습니다 - JavaScript 엔진은 컴파일 중에 선언을 파싱하고 선언과 해당 스코프를 인식합니다. 선언을 해당 스코프의 맨 위로 옮겨지는 것으로 생각하여 동작을 이해하는 것이 더 쉬울 뿐입니다. 몇 가지 예를 들어 설명해 보겠습니다.

  ```js
  // var 선언이 호이스팅됩니다
  console.log(foo); // undefined
  var foo = 1;
  console.log(foo); // 1

  // let/const 선언은 호이스팅되지 않습니다.
  console.log(bar); // ReferenceError: bar is not defined
  let bar = 2;
  console.log(bar); // 2
  ```

  함수 선언은 함수몸체가 호이스팅되는 반면, 변수 선언 형태로 작성된 함수 표현식은 변수 선언만 호이스팅됩니다.

  ```js
  // 함수 선언
  console.log(foo); // [Function: foo]
  foo(); // 'FOOOOO'
  function foo() {
    console.log("FOOOOO");
  }
  console.log(foo); // [Function: foo]

  // 함수 표현식
  console.log(bar); // undefined
  bar(); // Uncaught TypeError: bar is not a function
  var bar = function () {
    console.log("BARRRR");
  };
  console.log(bar); // [Function: bar]
  ```

* **이벤트 버블링(Event Bubbling)에 대해서 설명하세요.**

  DOM 요소에서 이벤트가 트리거되면 리스너가 연결되어 있는 경우 이벤트 처리를 시도한 다음, 해당 이벤트가 부모에게 bubbling되고 부모에서 같은 이벤트가 발생합니다. 이 bubbling은 요소의 최상단 부모요소인 `document`까지 계속적으로 발생시킵니다. 이벤트 bubbling은 이벤트 위임의 작동 메커니즘입니다.

- **이벤트 캡쳐링(Event Capturing)에 대해서 설명하세요.**

* **"속성(Attribute)"와 "요소(property)"의 차이가 무엇인가요?**

  attribute는 HTML 마크업에 정의되지만 property는 DOM에 정의됩니다. 차이점을 설명하기 위해 HTML에 다음 텍스트 필드가 있다고 가정해 봅시다: ``.

  ```js
  const input = document.querySelector("input");
  console.log(input.getAttribute("value")); // Hello
  console.log(input.value); // Hello
  ```

  그러나 텍스트 필드에 "World!"를 추가하면 이렇게 될것입니다.

  ```js
  console.log(input.getAttribute("value")); // Hello
  console.log(input.value); // Hello World!
  ```

  ###### 참고자료

  - https://stackoverflow.com/questions/6003819/properties-and-attributes-in-html

- **내장된 JavaScript 객체를 확장하는 것이 좋지 않은 이유는 무엇인가요?**

  내장/네이티브 JavaScript 객체를 확장한다는 것은 prototype에 속성/함수를 추가한다는 것을 의미합니다. 이것은 처음에는 좋은 생각처럼 보일 수 있지만 실제로는 위험합니다. 여러분의 코드가 동일한 `contains` 메소드를 추가함으로써 `Array.prototype`을 확장하는 여러가지 라이브러리를 사용한다고 상상해보십시오. 이러한 구현은 메소드를 서로 덮어쓰게 되며, 이 두 메소드의 동작이 동일하지 않으면 코드가 망가질 것입니다.

  네이티브 객체를 확장할 수 있는 유일한 경우는 polyfill을 만들 때입니다. JavaScript 사양의 일부이지만, 오래된 브라우저이기 때문에 사용자 브라우저에 없을 수도 있는 메서드에 대한 고유한 구현을 제공해야할 경우 뿐입니다.

  ###### 참고자료

  - http://lucybain.com/blog/2014/js-extending-built-in-objects/

* **document load event와 DOMContentLoaded event의 차이점은 무엇인가요?**

  `DOMContentLoaded` 이벤트는 스타일시트, 이미지, 서브프레임 로딩을 기다리지 않고, 초기 HTML 문서가 완전히 로드되고 파싱되면 발생합니다.

  `window`의 `load` 이벤트는 DOM과 모든 종속 리소스와 에셋들이 로드된 후에 발생합니다.

- **`==`와 `===`의 차이점은 무엇인가요?**

  `==`는 추상 동등 연산자이고 `===`는 완전 동등 연산자입니다. `==`연산자는 타입 변환이 필요한 경우 타입 변환을 한 후에 동등한지 비교할 것입니다. `===`연산자는 타입 변환을 하지 않으므로 두 값이 같은 타입이 아닌 경우 `===`는 `false`를 반환합니다. `==`를 사용하면 다음과 같은 무서운 일이 발생할 수 있습니다.

  ```js
  1 == "1"; // true
  1 == [1]; // true
  1 == true; // true
  0 == ""; // true
  0 == "0"; // true
  0 == false; // true
  ```

  저의 조언은 편의상 `null`과 `undefined`를 비교할 때를 제외하고, `==`연산자를 절대 사용하지 않는 것입니다. `a == null`은 `a`가 `null` 또는 `undefined`이면 `true`를 반환합니다.

  ```js
  var a = null;
  console.log(a == null); // true
  console.log(a == undefined); // true
  ```

  ###### 참고자료

  - https://stackoverflow.com/questions/359494/which-equals-operator-vs-should-be-used-in-javascript-comparisons

* **JavaScript의 "동일출처정책(the same-origin policy)"에 대해서 설명하세요.**

  same-origin 정책은 JavaScript가 도메인 경계를 넘어서 요청하는 것을 방지합니다. origin은 URI 체계, 호스트 이름, 포트 번호의 조합으로 정의됩니다. 이 정책은 한 페이지의 악의적인 스크립트가 해당 페이지의 DOM을 통해 다른 웹 페이지의 중요한 데이터에 접근하는 것을 방지합니다.

  ###### 참고자료

  - https://en.wikipedia.org/wiki/Same-origin_policy

- **다음 코드를 동작하게 만드세요.**

  ```js
  duplicate([1, 2, 3, 4, 5]); // [1,2,3,4,5,1,2,3,4,5]
  ```

  ```js
  duplicate([1, 2, 3, 4, 5]); // [1,2,3,4,5,1,2,3,4,5]
  function duplicate(arr) {
    return arr.concat(arr);
  }

  duplicate([1, 2, 3, 4, 5]); // [1,2,3,4,5,1,2,3,4,5]
  ```

* **삼항식(Ternary statement)을 사용하는 이유는 무엇이고, 그것을 표현하기 위한 연산자 단어는 무엇인가요?**

  "Ternary"는 "삼항"을 나타내고 삼항 표현식은 세가지 피연산자, 테스트 조건문, "then"표현식, "else"표현식을 받습니다. 삼항 표현식은 JavaScript에만 해당되는 것이 아니며 왜 이 목록에 있는지 잘 모르겠습니다.

  ###### 참고자료

  - https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Operators/Conditional_Operator

- **`use strict;`은 무엇이고, 사용했을 때 장단점에 관해서 설명해주세요.**

  'use strict'는 전체 스크립트나 개별 함수에 엄격 모드를 사용하는데 사용되는 명령문입니다. Strict 모드는 JavaScript 다양한 자바스크립트를 제한하는 방법입니다.

  장점:

  - 실수로 전역변수를 만드는 것이 불가능합니다.
  - 암묵적으로 실패한 예외를 throw하지 못하는 할당을 만듭니다.
  - 삭제할 수 없는 속성을 삭제하려고 시도합니다. (시도 효과가 없을 때까지)
  - 함수의 매개변수 이름은 고유해야합니다.
  - `this`는 전역 컨텍스트에서 undefined입니다.
  - 예외를 발생시키는 몇 가지 일반적인 코딩을 잡아냅니다.
  - 헷갈리거나 잘 모르는 기능을 사용할 수 없게 합니다.

  단점:

  - 일부 개발자는 익숙하지 않은 기능이 많습니다.
  - `function.caller`와 `function.arguments`에 더 이상 접근할 수 없습니다.
  - 서로 다른 엄격한 모드로 작성된 스크립트를 병합하면 문제가 발생할 수 있습니다.

  전반적으로 장점이 단점보다 중요하다고 생각합니다. 엄격 모드가 차단하는 기능에 의존하지 않아도 됩니다. 엄격한 모드를 사용하는 것을 추천합니다.

  ###### 참고자료

  - http://2ality.com/2011/10/strict-mode-hatred.html
  - http://lucybain.com/blog/2014/js-use-strict/

* **100번 반복되는 반복문이 있습니다. 3의 배수일 때는 `fizz`, 5의 배수일 때는 `buzz`, 3과 5의 공배수일 때는 `fizzbuzz`가 출력되는 코드를 작성해보세요.**

  [Paul Irish](https://gist.github.com/jaysonrowe/1592432#gistcomment-790724)의 FizzBuzz를 확인해보세요.

  ```js
  for (let i = 1; i <= 100; i++) {
    let f = i % 3 == 0,
      b = i % 5 == 0;
    console.log(f ? (b ? "FizzBuzz" : "Fizz") : b ? "Buzz" : i);
  }
  ```

  저는 인터뷰 중에 위와 같이 쓰라고 조언하지는 않습니다. 길지만 분명한 접근 방식을 고수하세요. FizzBuzz의 더 다양한 버전을 보려면 아래의 참조 링크를 확인하세요.

  ###### 참고자료

  - https://gist.github.com/jaysonrowe/1592432

- **일반적으로 웹 사이트의 전역 스코프를 그대로 두고 건드리지 않는 것이 좋은 이유는 무엇인가요?**

  모든 스크립트는 전역 스코프에 접근할 수 있으며, 모든 사람이 전역 네임스페이스를 사용하여 변수를 정의하면 충돌이 발생할 수 있습니다. 모듈 패턴 (IIFEs)을 사용하여 변수를 로컬 네임스페이스 내에 캡슐화하세요.

* **때때로 `load` event를 사용하는 이유에 관해 설명해주세요. 또 단점이 있다면 대안에 대해서도 설명해주세요.**

  `load` 이벤트는 문서로딩 프로세스가 끝날 때 발생됩니다. 이 시점에서 문서의 모든 객체가 DOM에 있고, 모든 이미지, 스크립트, 링크 및 하위 프레임로딩이 완료됩니다.

  DOM 이벤트 `DOMContentLoaded`는 페이지의 DOM이 생성된 후에 발생하지만 다른 리소스가 로딩되기를 기다리지 않습니다. 이것은 초기화되기 전에 전체 페이지가 로드될 필요가 없는 경우에 선호됩니다.

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/API/GlobalEventHandlers/onload

- **single page app이 무엇인지 설명하고 SEO-friendly하게 만드는 방법을 설명하세요.**

  아래는 [Grab Front End Guide](https://github.com/grab/front-end-guide)에서 가져온 것이며, 우연히도 제가 작성했습니다!

  웹 개발자는 요즘 웹 사이트가 아닌 웹 앱으로 제작한 제품을 언급합니다. 두 가지 용어 사이에는 엄격한 차이는 없지만, 웹 앱은 대화형, 동적인 경향이 있어 사용자가 작업을 수행하고 작업에 대한 응답을 받을 수 있습니다. 전통적으로, 브라우저는 서버에서 HTML을 받아 렌더링합니다. 사용자가 다른 URL로 이동하면, 전체페이지 새로고침이 필요하며 서버는 새페이지에 대해 새 HTML을 보냅니다. 이를 server-side rendering이라고합니다.

  그러나 현대 SPA에서는 대신 client-side rendering이 사용됩니다. 브라우저는 전체 애플리케이션에 필요한 스크립트(프레임워크, 라이브러리, 앱 코드) 및 스타일시트와 함께 서버의 초기 페이지를 로드합니다. 사용자가 다른 페이지로 이동하면 페이지 새로고침이 발생하지 않습니다. 페이지의 URL은 [HTML5 History API](https://developer.mozilla.org/en-US/docs/Web/API/History_API)를 통해 업데이트됩니다. 일반적으로 JSON 형식의 새 페이지에 필요한 새 데이터는 브라우저에서 [AJAX](https://developer.mozilla.org/en-US/docs/AJAX/Getting_Started) 요청을 통해 서버로 전송됩니다. SPA는 초기 페이지 로딩에서 미리 다운로드된 JavaScript를 통해 페이지를 동적으로 업데이트합니다. 이 모델은 네이티브 모바일 앱의 작동 방식과 유사합니다.

  장점들:

  - 전체 페이지 새로고침으로 인해 페이지 탐색 사이에 하얀 화면이 보이지 않아 앱이 더 반응적으로 느껴지게 됩니다.
  - 동일한 애셋을 페이지 로드마다 다시 다운로드할 필요가 없으므로 서버에 대한 HTTP 요청이 줄어듭니다.
  - 클라이언트와 서버 사이의 고려해야 할 부분을 명확하게 구분합니다. 서버 코드를 수정하지 않고도 다양한 플랫폼(예: 모바일, 채팅 봇, 스마트워치)에 맞는 새로운 클라이언트를 쉽게 구축할 수 있습니다. 또한 API 규약이 깨지지 않는 한도 내에서 클라이언트와 서버에서 기술 스택을 독립적으로 수정할 수 있습니다.

  단점들:

  - 여러 페이지에 필요한 프레임워크, 앱 코드, 애셋로드로 인해 초기 페이지로드가 무거워집니다.
  - 모든 요청을 단일 진입점으로 라우트하고 클라이언트 측 라우팅이 그 한곳에서 인계받을 수 있도록 서버를 구성하는 추가 단계가 필요합니다.
  - SPA는 콘텐츠를 렌더링하기 위해 JavaScript에 의존하지만 모든 검색 엔진이 크롤링 중에 JavaScript를 실행하지는 않으며 페이지에 빈 콘텐츠가 표시될 수 있습니다. 이로 인해 의도치 않게 앱의 검색 엔진 최적화(SEO)가 어려워집니다.
    그러나 대부분의 경우 앱을 제작할 때 검색 엔진에서 모든 콘텐츠 색인할 필요는 없으므로 SEO가 가장 중요한 요소는 아닙니다. 이를 극복하기 위해, 앱을 서버 측 렌더링하거나 [Prerender](https://prerender.io/)와 같은 서비스를 사용하여 "브라우저에서 JavaScript를 렌더링하고, 정적 HTML을 저장한 다음, 크롤러에게 반환합니다".

  ###### 참고자료

  - https://github.com/grab/front-end-guide#single-page-apps-spas
  - http://stackoverflow.com/questions/21862054/single-page-app-advantages-and-disadvantages
  - http://blog.isquaredsoftware.com/presentations/2016-10-revolution-of-web-dev/
  - https://medium.freecodecamp.com/heres-why-client-side-rendering-won-46a349fadb52

* **Promise를 사용해 본 경험이 있나요?**

  Promise는 어느 시점에 resolve된 값 또는 resolve되지 않은 이유(예: 네트워크 오류가 발생) 중 하나의 값을 생성할 수 있는 객체입니다. promise는 fulfilled, rejected, pending 3가지 상태 중 하나일 수 있습니다. promise 사용자는 콜백을 붙여서 fulfill된 값이나 reject된 이유를 처리할 수 있습니다.

  일반적인 polyfill은 `$.deferred`, Q, Bluebird 입니다만, 모두가 스펙을 따르는 것은 아닙니다. ES2015는 즉시 사용할 수 있는 Promise를 지원하며 일반적으로 요즘엔 polyfill이 필요하지 않습니다.

  ###### 참고자료

  - https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-promise-27fc71e77261

- **Callback 대신에 Promise를 사용할 때의 장점과 단점은 무엇인가요?**

  **장점**

  - 가독성이 떨어질 수 있는 콜백 지옥을 피할 수 있습니다.
  - `.then()`을 이용하여 가독성 좋은 연속적인 비동기 코드를 쉽게 작성할 수 있습니다.
  - `Promise.all()`을 사용하여 병렬 비동기 코드를 쉽게 작성할 수 있습니다.
  - Promise를 통해 콜백만 사용하는 코딩방식에 있는 다음과 같은 상황이 발생하지 않습니다:
    - 콜백을 너무 빨리 호출함
    - 콜백을 너무 늦게 호출하거나 호출하지 않음
    - 콜백을 너무 적게 호출하거나 너무 많이 호출함
    - 필요한 환경/매개변수를 전달하는데 실패함
    - 발생가능한 오류/예외를 무시함

  **단점**

  - 약간 더 복잡한 소스코드(논쟁의 여지가 있음).
  - ES2015를 지원하지 않는 이전 브라우저에서 이를 사용하기 위해서는 polyfill을 로드해야 합니다.

  ###### 참고자료

  - [https://github.com/getify/You-Dont-Know-JS/blob/master/async%20%26%20performance/ch3.md](https://github.com/getify/You-Dont-Know-JS/blob/master/async %26 performance/ch3.md)

* **JavaScript의 작동방식의 장단점에 관해 설명해주세요.**

  JavaScript로 컴파일되는 언어의 예로 CoffeeScript, Elm, ClojureScript, PureScript, TypeScript가 있습니다.

  **장점:**

  - JavaScript의 오랜 문제점들을 해결하고 JavaScript 안티-패턴을 방지합니다.
  - JavaScript 위에 syntatic sugar를 제공함으로써 더 짧은 소스코드를 작성할 수 있도록 해줍니다. 제 생각에는 ES5는 부족하지만 ES2015는 굉장합니다.
  - 정적 타입은 시간 경과에 따라 유지 관리해야 하는 대규모 프로젝트에서 훌륭합니다(TypeScript의 경우).

  **단점:**

  - 브라우저는 오직 JavaScript만 실행하기 때문에 빌드/컴파일 프로세스가 필요하며 브라우저에 제공되기 전에 JavaScript로 코드를 컴파일해야 합니다.
  - 소스 맵이 미리 컴파일된 소스에 잘 매핑되지 않으면 디버깅이 어려울 수 있습니다.
  - 대부분의 개발자들은 이러한 언어에 익숙하지 않으므로 이를 배워야합니다. 프로젝트에 사용할 경우 팀 비용이 증가합니다.
  - 소규모 커뮤니티(언어에 따라 다름)에서는 리소스, 튜토리얼, 라이브러리, 툴을 찾기가 어려울 수 있습니다.
  - IDE / 편집기 지원이 부족할 수 있습니다.
  - 이러한 언어는 항상 최신 JavaScript 표준보다 뒤쳐질 것입니다.
  - 개발자들은 자신들의 코드를 무엇으로 컴파일하고 있는지 알고 있어야 합니다. 왜냐하면 그것이 실제로 실행될 것이고, 그것이 결국 중요하기 때문입니다.

  실질적으로 ES2015는 JavaScript를 크게 개선하여 작성하기가 훨씬 쉬워졌습니다. 요즘은 CoffeeScript가 필요성을 느끼지 못합니다.

  ###### 참고자료

  - https://softwareengineering.stackexchange.com/questions/72569/what-are-the-pros-and-cons-of-coffeescript

- **JavaScript를 디버깅할 때 사용하는 도구가 있으면 설명해주세요.**

  - React and Redux
    - [React Devtools](https://github.com/facebook/react-devtools)
    - [Redux Devtools](https://github.com/gaearon/redux-devtools)
  - JavaScript
    - [Chrome Devtools](https://hackernoon.com/twelve-fancy-chrome-devtools-tips-dc1e39d10d9d)
    - `debugger` statement
    - Good old `console.log` debugging

  ###### 참고자료

  - https://hackernoon.com/twelve-fancy-chrome-devtools-tips-dc1e39d10d9d
  - https://raygun.com/blog/javascript-debugging/

* **객체 안의 속성과 배열의 아이템을 순회할 때 사용하는 문법에 관해 설명해주세요.**

  **오브젝트의 경우:**

  - `for-in` 반복 - `for (var property in obj) { console.log(property); }`. 그러나, 이는 상속된 속성도 반복되며, 사용하기 전에 `obj.hasOwnProperty(property)` 체크를 추가해야 합니다.
  - `Object.keys()` - `Object.keys(obj).forEach(function (property) { ... })`. `Object.keys()`는 전달하는 객체의 열거 가능한 모든 속성을 나열하는 정적 메서드입니다.
  - `Object.getOwnPropertyNames()` - `Object.getOwnPropertyNames(obj).forEach(function (property) { ... })`. `Object.getOwnPropertyNames()`는 전달하는 객체의 열거 가능한 속성과 열거불가능한 모든 속성을 나열하는 정적 메서드입니다.

  **배열의 경우:**

  - `for` 반복 - `for (var i = 0; i < arr.length; i++)`. 여기에 있는 일반적인 함정은 `var`이 함수 스코프고 블록 스코프가 아니며, 대부분 블록 스코프의 반복자 변수를 원할 것이라는 점입니다. ES2015에는 블록 범위가 있는 `let`이 추가됐고, 이를 대신 사용할 것을 권장합니다. 그래서 다음과 같이 됩니다. `for (let i = 0; i < arr.length; i++)`.
  - `forEach` - `arr.forEach(function (el, index) { ... })`. 필요한 것이 배열의 요소라면 `index`를 사용할 필요가 없기 때문에 이 구문이 더 편리 할 수 있습니다. 또한 `every`과 `some`메서드를 이용하여 반복을 일찍 끝낼 수 있습니다.
  - `for-of` 반복 - `for (let elem of arr) { ... }`. ES6는 `String`, `Array`, `Map`, `Set` 등과 같은 [iterable protocol](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Iteration_protocols#The_iterable_protocol)을 준수하는 객체를 반복 할 수 있게 해주는 새로운 `for-of` 루프를 도입했습니다. `for` 루프의 장점은 루프에서 벗어날 수 있다는 것이고, `forEach()`의 장점은 카운터 변수가 필요 없기 때문에 `for` 루프보다 간결하다는 것입니다. `for-of` 루프를 사용하면, 루프에서 빠져 나올 수도 있고 더 간결한 구문도 얻을 수 있습니다.

  대부분의 경우에 저는 `.forEach` 메서드를 선호하지만, 무엇을 하느냐에 따라서 각 상황에 맞게 사용하는 것이 좋습니다. ES6 이전에는 `for` 루프를 사용하여 루프를 조기 종료해야 할 때 `break`를 사용했습니다. 그러나 이제 ES6에서는 `for-of`루프를 사용하여 이를 수행 할 수 있습니다. 루프 당 반복자를 두 번 이상 늘리는 것과 같이 유연성이 더 필요하다면, `for` 루프를 사용할 것입니다.

  또한, `for-of` 루프를 사용할 때 각 배열 요소의 인덱스와 값에 모두 접근해야하는 경우 ES6 Array의 `entries()` 메소드와 destructuring을 사용하면됩니다.

  ```js
  const arr = ["a", "b", "c"];

  for (let [index, elem] of arr.entries()) {
    console.log(index, ": ", elem);
  }
  ```

  ###### 참고자료

  - http://2ality.com/2015/08/getting-started-es6.html#from-for-to-foreach-to-for-of
  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/entries

- mutable object와 immutable object에 관해 설명해주세요.
  - JavaScript에서 immutable 객체의 예를 들어보세요.
  - immutability의 장/단점은 무엇인가요?
  - 자신의 코드에서 불변성(immutability를) 어떻게 달성할 수 있나요?

* **동기방식과 비동기 방식 함수의 차이에 관해서 설명해주세요.**

  동기 함수는 블로킹인 반면, 비동기 함수는 그렇지 않습니다. 동기 함수에서는 다음 명령문이 실행되기 전에 앞 명령문이 완료됩니다. 이 경우, 프로그램은 명령문의 순서대로 정확하게 평가되고 명령문 중 하나가 매우 오랜 시간이 걸리면 프로그램 실행이 일시중지됩니다.

  비동기 함수는 일반적으로 파라미터를 통해서 콜백을 받고, 비동기 함수가 호출된 후 즉시 다음 줄 실행이 계속됩니다. 콜백은 비동기 작업이 완료되고 호출 스택이 비어 있을 때만 호출됩니다. 웹 서버에서 데이터를 로드하거나 데이터베이스를 쿼리하는 등의 무거운 작업을 비동기식으로 수행하여, 메인 스레드가 긴 작업을 완료할 때까지 블로킹하지 않고 다른 작업을 계속할 수 있습니다(브라우저의 경우 UI가 중지됨).

- **이벤트 루프란 무엇인가요? 콜 스택과 태스크 큐의 차이점은 무엇인가요?call stack과 task queue에 관해 설명해주세요.**

  이벤트 루프는 콜 스택을 모니터하고 태스크 큐에서 수행할 작업이 있는지 확인하는 단일 스레드 루프입니다. 콜 스택이 비어 있고 태스크 큐에 콜백 함수가 있는 경우, 함수는 큐에서 제거되고 실행될 콜 스택으로 푸시됩니다.

  Philip Robert의 [talk on the Event Loop](https://2014.jsconf.eu/speakers/philip-roberts-what-the-heck-is-the-event-loop-anyway.html)를 아직 확인하지 않은 경우 확인하십시오. JavaScript 분야에서 가장 많은 조회수를 기록한 동영상 중 하나입니다.

  ###### 참고자료

  - https://2014.jsconf.eu/speakers/philip-roberts-what-the-heck-is-the-event-loop-anyway.html
  - http://theproactiveprogrammer.com/javascript/the-javascript-event-loop-a-stack-and-a-queue/

* **`function foo() {}`와 `var foo = function() {}`에서 foo 의 차이가 무엇인지 설명해보세요.**

  전자는 함수 선언인 반면, 후자는 함수 표현식입니다. 주요한 차이점은 함수 선언은 함수바디가 호이스트되지만, 함수 표현식의 바디는 호이스트되지 않습니다(변수와 동일한 호이스팅 동작을 가짐). 호이스팅에 대한 자세한 설명은 질문 위의 호이스팅을 참조하십시오. 함수 표현식을 정의하기 전에 호출하려고 하면 `Uncaught TypeError : XXX is not function` 에러가 발생합니다.

  **함수 선언**

  ```js
  foo(); // 'FOOOOO'
  function foo() {
    console.log("FOOOOO");
  }
  ```

  **함수 표현식**

  ```js
  foo(); // Uncaught TypeError: foo는 함수가 아닙니다
  var foo = function () {
    console.log("FOOOOO");
  };
  ```

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function

- `let`, `var`, `const`의 차이점에 관해서 설명해주세요.

  ### `let`, `var`, `const`를 사용하여 생성된 변수들의 차이점은 무엇인가요?

  `var` 키워드를 사용하여 선언된 변수는 함수가 생성된 함수나 함수 밖에서 생성된 함수에 전역 오브젝트로 적용됩니다. `let`과 `const`는 블록 스코프입니다. 즉, 가장 가까운 중괄호(function, if-else 블록, for-loop) 내에서만 접근할 수 있습니다.

  ```js
  function foo() {
    // 함수 내에서 모든 변수에 접근할 수 있습니다.
    var bar = "bar";
    let baz = "baz";
    const qux = "qux";

    console.log(bar); // "bar"
    console.log(baz); // "baz"
    console.log(qux); // "qux"
  }

  console.log(bar); // ReferenceError: bar is not defined
  console.log(baz); // ReferenceError: baz is not defined
  console.log(qux); // ReferenceError: qux is not defined
  if (true) {
    var bar = "bar";
    let baz = "baz";
    const qux = "qux";
  }

  // var로 선언된 변수는 함수 스코프의 어디에서나 접근할 수 있습니다.
  console.log(bar); // "bar"
  // let과 const로 정의된 변수는 정의된 블록 외부에서 접근할 수 없습니다.
  console.log(baz); // ReferenceError: baz is not defined
  console.log(qux); // ReferenceError: qux is not defined
  ```

  `var`는 변수가 호이스트되도록 허용합니다. 즉, 변수가 선언되기 전에 코드에서 참조될 수 있습니다. `let`과 `const`는 이를 허용하지 않고 대신 에러를 던집니다.

  ```js
  console.log(foo); // undefined

  var foo = "foo";

  console.log(baz); // ReferenceError: can't access lexical declaration 'baz' before initialization

  let baz = "baz";

  console.log(bar); // ReferenceError: can't access lexical declaration 'bar' before initialization

  const bar = "bar";
  ```

  `var`을 사용하여 변수를 다시 선언해도 에러가 발생하지 않지만, `let`과 `const`는 에러를 발생시킵니다.

  ```js
  var foo = "foo";
  var foo = "bar";
  console.log(foo); // "bar"

  let baz = "baz";
  let baz = "qux"; // Uncaught SyntaxError: Identifier 'baz' has already been declared
  ```

  `let`은 변수의 값을 재할당할 수 있지만, `const`는 재할당할 수 없다는 점이 다릅니다.

  ```js
  // 괜찮습니다
  let foo = "foo";
  foo = "bar";

  // 예외가 발생합니다
  const baz = "baz";
  baz = "qux";
  ```

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let
  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var
  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const

* **ES6 클래스와 ES5 함수 생성자의 차이점은 무엇인가요?**

  먼저 각각의 예를 살펴보겠습니다.

  ```js
  // ES5 함수 생성자
  function Person(name) {
    this.name = name;
  }

  // ES6 클래스
  class Person {
    constructor(name) {
      this.name = name;
    }
  }
  ```

  간단한 생성자의 경우에는 매우 유사합니다.

  생성자의 주요 차이점은 상속을 사용할 때 발생합니다. `Person`의 하위 클래스이면서 `studentId` 필드를 추가로 가지고 있는 `Student` 클래스를 만들고자 한다면, 이것이 우리가 추가로 해야할 일입니다.

  ```js
  // ES5 함수 생성자
  function Student(name, studentId) {
    // 수퍼 클래스의 생성자를 호출하여 수퍼 클래스에서 상속된 멤버를 초기화합니다.
    Person.call(this, name);

    // 서브 클래스의 멤버를 초기화합니다.
    this.studentId = studentId;
  }

  Student.prototype = Object.create(Person.prototype);
  Student.prototype.constructor = Student;

  // ES6 클래스
  class Student extends Person {
    constructor(name, studentId) {
      super(name);
      this.studentId = studentId;
    }
  }
  ```

  ES5에서 상속을 사용하는 것이 훨씬 더 불편하며, ES6 버전이 이해하고 기억하기가 더 쉽습니다.

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Inheritance
  - https://eli.thegreenplace.net/2013/10/22/classical-inheritance-in-javascript-es5

- **새 화살표 => 함수 문법에 대한 사용 예시를 들 수 있나요? 이 새로운 문법은 다른 함수와 어떻게 다른가요?**

  화살표 함수의 한 가지 분명한 이점은 `function` 키워드를 사용하지 않고도 함수를 생성하는데 필요한 문법을 단순화하는 것입니다.

  또한, 화살표 함수 내의 `this`는, `this`가 함수를 호출하는 객체에 의해 결정되는 일반 함수와 다르게, 주변 스코프에에 묶입니다.

  렉시컬스코프 `this`는 특히 React 컴포넌트에서 콜백을 호출할 때 유용합니다.

* **생성자의 메서드에 화살표 문법을 사용하면 어떤 이점이 있나요?**

  생성자 내부에서 화살표 함수를 메소드로 사용하는 주된 장점은, 함수 생성시 `this`의 값이 설정되고 그 이후에는 변경할 수 없다는 것입니다.

  따라서, 생성자가 새로운 객체를 생성하는데 사용될 때, `this`는 항상 그 객체를 참조할 것입니다.

  예를 들어, 우리가 인수로 first name을 받고, 그 이름을 `console.log`로 출력하는 `Person` 생성자가 있다고 해봅시다. 하나는 일반 함수이고, 다른 하나는 화살표 함수일 때,

  ```js
  const Person = function (firstName) {
    this.firstName = firstName;
    this.sayName1 = function () {
      console.log(this.firstName);
    };
    this.sayName2 = () => {
      console.log(this.firstName);
    };
  };

  const john = new Person("John");
  const dave = new Person("Dave");

  john.sayName1(); // John
  john.sayName2(); // John

  // 일반 함수의 'this'값은 변경할 수 있지만, 화살표 함수는 변경할 수 없습니다.
  john.sayName1.call(dave); // Dave (because "this" is now the dave object)
  john.sayName2.call(dave); // John

  john.sayName1.apply(dave); // Dave (because 'this' is now the dave object)
  john.sayName2.apply(dave); // John

  john.sayName1.bind(dave)(); // Dave (because 'this' is now the dave object)
  john.sayName2.bind(dave)(); // John

  var sayNameFromWindow1 = john.sayName1;
  sayNameFromWindow1(); // undefined (because 'this' is now the window object)

  var sayNameFromWindow2 = john.sayName2;
  sayNameFromWindow2(); // John
  ```

  여기에서 주요 장점은 `this`는 일반 함수에 대해 변경될 수 있지만, 컨텍스트는 항상 화살표 함수에 대해 동일하게 유지된다는 것입니다. 따라서 화살표 함수를 앱의 다른 부분으로 전달하는 경우에도 컨텍스트 변경에 대해 걱정할 필요가 없습니다.

  이는 특히 React 클래스 컴포넌트에서 유용할 수 있습니다. 일반 함수를 사용하는 클릭 핸들러와 같은 클래스 메소드를 정의한 다음, 해당 클릭 핸들러를 하위 컴포넌트의 prop으로 전달하면 상위 컴포넌트의 생성자에서 `this`도 바인드해야합니다.

  대신 화살표 함수를 사용하면, 메소드가 `this`값을 주위 렉시컬 컨텍스트에서 자동으로 가져오기 때문에 `this`를 바인딩할 필요가 없습니다.

  (좋은 데모, 샘플 코드는 [이 기사](https://medium.com/@machnicki/handle-events-in-react-with-arrow-functions-ede88184bbb)를 참조하세요.)

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions
  - https://medium.com/@machnicki/handle-events-in-react-with-arrow-functions-ede88184bbb

- **고차 함수(higher-order function)의 정의는 무엇인가요?**

  고차 함수는 다른 함수를 매개 변수로 사용하여 어떤 데이터를 처리하거나, 결과로 함수를 반환하는 함수입니다. 고차 함수는 반복적으로 수행되는 어떤 연산을 추상화하기 위한 것입니다. 전형적인 예시는 배열과 함수를 인수로 취하는 `map`입니다. `map`은 고차 함수를 사용하여 배열의 각 항목을 변환하고, 변환된 데이터로 새로운 배열을 반환합니다. JavaScript에서 흔히 볼 수 있는 다른 예로 `forEach`, `filter`, `reduce`가 있습니다. 다른 함수에서 함수를 반환하는 많은 사용사례가 있기 때문에 고차 함수는 배열을 조작할 필요가 없습니다. `Array.prototype.bind`는 JavaScript에서 그러한 예시 중 하나입니다.

  **Map**

  각 요소를 대문자 문자열로 변환해야하는 이름들을 가진 배열이 있다고 가정해 보겠습니다.

  ```js
  const names = ["irish", "daisy", "anna"];
  ```

  일반적인 방법은 다음과 같습니다.

  ```js
  const transformNamesToUppercase = function (names) {
    const results = [];
    for (let i = 0; i < names.length; i++) {
      results.push(names[i].toUpperCase());
    }
    return results;
  };
  transformNamesToUppercase(names); // ['IRISH', 'DAISY', 'ANNA']
  ```

  `.map(transformerFn)`을 사용하면 코드가 더 짧아지고 선언적이어집니다.

  ```js
  const transformNamesToUppercase = function (names) {
    return names.map((name) => name.toUpperCase());
  };
  transformNamesToUppercase(names); // ['IRISH', 'DAISY', 'ANNA']
  ```

  ###### 참고자료

  - https://medium.com/javascript-scene/higher-order-functions-composing-software-5365cf2cbe99
  - https://hackernoon.com/effective-functional-javascript-first-class-and-higher-order-functions-713fde8df50a
  - https://eloquentjavascript.net/05_higher_order.html

* **객체나 배열에 대한 디스트럭쳐링 예시를 들 수 있나요?**

  디스트럭쳐링은 ES6에서 사용할 수 있는 표현식으로 객체나 배열의 값을 추출하여 다른 변수에 배치하는 간결하고 편리한 방법을 제공합니다.

  **배열 디스트럭쳐링**

  ```js
  // 변수 할당.
  const foo = ["one", "two", "three"];

  const [one, two, three] = foo;
  console.log(one); // "one"
  console.log(two); // "two"
  console.log(three); // "three"
  // 변수 교환
  let a = 1;
  let b = 3;

  [a, b] = [b, a];
  console.log(a); // 3
  console.log(b); // 1
  ```

  **객체 디스트럭쳐링**

  ```js
  // 변수 할당.
  const o = { p: 42, q: true };
  const { p, q } = o;

  console.log(p); // 42
  console.log(q); // true
  ```

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment
  - https://ponyfoo.com/articles/es6-destructuring-in-depth

- **ES6 템플릿 리터럴은 문자열을 생성하는데 많은 유연성을 제공합니다. 이에 대한 예를 들 수 있나요?**

  템플릿 리터럴을 사용하면 문자열 보간을 하거나 문자열에 변수를 포함하는 작업을 간단하게 수행할 수 있습니다. ES2015 이전에는 아래와 같이하는 것이 일반적이었습니다.

  ```js
  var person = { name: "Tyler", age: 28 };
  console.log(
    "Hi, my name is " + person.name + " and I am " + person.age + " years old!"
  );
  // 'Hi, my name is Tyler and I am 28 years old!'
  ```

  템플릿 리터럴을 사용하면, 대신 이렇게해도 같은 출력을 만들 수 있습니다.

  ```js
  const person = { name: "Tyler", age: 28 };
  console.log(
    `Hi, my name is ${person.name} and I am ${person.age} years old!`
  );
  // 'Hi, my name is Tyler and I am 28 years old!'
  ```

  템플릿 리터럴을 사용하고 있으며 `${}` 플레이스홀더 안에 표현식을 삽입할 수 있다는 것을 나타내기 위해 따옴표(`'`)가 아닌 백틱(`)을 사용한다는 것에 유의하세요.

  두번째 유용한 사용사례는 다중행 문자열을 만드는 것입니다. ES2015 이전에는 아래와 같이 다행의 문자열을 만들 수 있었습니다.

  ```js
  console.log("This is line one.\nThis is line two.");
  // This is line one.
  // This is line two.
  ```

  또는 코드에서 여러 줄로 나눠진 긴 문자열을 읽기 위해 텍스트 편집기에서 오른쪽으로 스크롤 할 필요가 없도록하려면 다음과 같이 작성할 수 있습니다.

  ```js
  console.log("This is line one.\n" + "This is line two.");
  // This is line one.
  // This is line two.
  ```

  그러나 템플릿 리터럴은 당신이 추가한 간격 그대로 유지됩니다. 예를 들어, 위에 작성한 것과 동일한 다중행 출력을 작성하려면 다음과 같이하면 됩니다.

  ```js
  console.log(`This is line one.
  This is line two.`);
  // This is line one.
  // This is line two.
  ```

  템플릿 리터럴의 또 다른 사용사례는 간단한 변수 보간을 위한 템플릿 라이브러리의 대체품으로 사용하는 것입니다.

  ```js
  const person = { name: "Tyler", age: 28 };
  document.body.innerHTML = `
    <div>
      <p>Name: ${person.name}</p>
      <p>Name: ${person.age}</p>
    </div>
  `;
  ```

  **`.innerHTML`을 사용하면 코드가 XSS의 영향을 받을 수 있습니다. 사용자로부터 입력받은 데이터인 경우 표시하기 전에 데이터를 안전하게 만드세요!**

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals

* **curry 함수의 예를 들어 줄 수 있나요? 그리고 이 문법은 어떤 이점을 가지고 있나요?**

  currying은 둘 이상의 매개 변수가 있는 함수가 여러 함수로 분리된 패턴으로, 직렬로 호출하면, 필요한 모든 매개 변수가 한 번에 하나씩 누적됩니다. 이 기법은 함수형 스타일로 작성된 코드를 읽고, 합성하기 더 쉬워진 경우 유용할 수 있습니다. 함수를 currying하려면, 하나의 함수로 시작하여, 하나의 매개 변수를 취하는 일련의 함수로 분리해야 합니다.

  ```js
  function curry(fn) {
    if (fn.length === 0) {
      return fn;
    }

    function _curried(depth, args) {
      return function (newArgument) {
        if (depth - 1 === 0) {
          return fn(...args, newArgument);
        }
        return _curried(depth - 1, [...args, newArgument]);
      };
    }

    return _curried(fn.length, []);
  }

  function add(a, b) {
    return a + b;
  }

  var curriedAdd = curry(add);
  var addFive = curriedAdd(5);

  var result = [0, 1, 2, 3, 4, 5].map(addFive); // [5, 6, 7, 8, 9, 10]
  ```

  ###### 참고자료

  - https://hackernoon.com/currying-in-js-d9ddc64f162e

- **spread 문법을 사용할 때의 이점은 무엇이며 rest 문법과 다른 점은 무엇인가요?**

  ES6의 spread 문법은 함수형 패러다임에서 코딩할 때 매우 유용합니다. 왜냐하면 `Object.create`, `slice`나 라이브러리 함수를 사용하지 않고도 배열이나 객체의 복사본을 쉽게 만들 수 있기 때문입니다. 이 언어 기능은 Redux나 Rx.js를 사용하는 프로젝트에서 많이 사용됩니다.

  ```js
  function putDookieInAnyArray(arr) {
    return [...arr, "dookie"];
  }

  var result = putDookieInAnyArray(["I", "really", "don't", "like"]); // ["I", "really", "don't", "like", "dookie"]

  var person = {
    name: "Todd",
    age: 29,
  };

  var copyOfTodd = { ...person };
  ```

  ES6의 rest 구문은 함수에 전달할 임의의 수의 인수를 포함하는 약식을 제공합니다. 이는 데이터의 배열을 채우기보다는 데이터를 가져와서 배열로 채우는 spread 구문의 반대와 비슷하며, 배열이나 객체 디스트럭쳐링 할당뿐만 아니라 함수 인수에서도 작동합니다.

  ```js
  function addFiveToABunchOfNumbers(...numbers) {
    return numbers.map((x) => x + 5);
  }

  const result = addFiveToABunchOfNumbers(4, 5, 6, 7, 8, 9, 10); // [9, 10, 11, 12, 13, 14, 15]

  const [a, b, ...rest] = [1, 2, 3, 4]; // a: 1, b: 2, rest: [3, 4]

  const { e, f, ...others } = {
    e: 1,
    f: 2,
    g: 3,
    h: 4,
  }; // e: 1, f: 2, others: { g: 3, h: 4 }
  ```

  ###### 참고자료

  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax
  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/rest_parameters
  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment

* **파일 간에 코드를 공유하려면 어떻게 해야하나요?**

  이것은 Javascript 환경에 따라 다릅니다.

  클라이언트(브라우저 환경)에서는, 변수/함수가 전역 스코프(`window`)에 선언되어있는 한 모든 스크립트가 이를 참조할 수 있습니다. 또는, 보다 모듈형 접근 방식을 위해 RequireJS를 통해 비동기 모듈 정의(AMD)를 이용합니다.

  서버(Node.js)에서 일반적인 방법은 CommanJS를 사용하는 것입니다. 각 파일은 모듈로 취급되며, 변수와 함수를 `module.exports` 객체에 붙여서 내보낼 수 있습니다.

  ES2015에서는 AMD 및 commonJS를 모두 대체하기 위한 모듈 문법을 정의합니다. 이 기능은 브라우저 및 노드 환경 모두에서 지원됩니다.

  ###### 참고자료

  - http://requirejs.org/docs/whyamd.html
  - https://nodejs.org/docs/latest/api/modules.html
  - http://2ality.com/2014/09/es6-modules-final.html

- **정적 클래스 멤버를 만드는 이유는 무엇인가요?**

  정적 클래스 멤버(속성/메서드)는 클래스의 특정 인스턴스와 묶이지 않으며, 어떤 인스턴스가 이를 참조하는지에 관계없이 동일한 값을 가집니다. 정적 속성은 일반적으로 설정(configuration) 변수이며 정적 메서드는 일반적으로 인스턴스의 상태에 의존하지 않는 순수 유틸리티 함수입니다.

  ###### 참고자료

  - https://stackoverflow.com/questions/21155438/when-to-use-static-variables-methods-and-when-to-use-instance-variables-methods

### References

- https://velog.io/@chris/front-end-interview-handbook-js-1
- https://velog.io/@chris/front-end-interview-handbook-js-2
- https://velog.io/@chris/front-end-interview-handbook-js-3
- https://velog.io/@chris/front-end-interview-handbook-js-4

---
