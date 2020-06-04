## Vue.js 가 뭔가요?
- Even You(에번 유) 가 2014년도에 발표한 자바스크립트 프레임워크
- 동적인 사용자 인터페이스(UI) 를 만들기 위한 프레임워크

## Vue instance 는 어떻게 생성하나요?
- Vue() 생성자 함수를 이용하여 생성
- 생성시 옵션 객체를 전달
let vm = new Vue({});
- vue component 도 vue instance 와 동일하다.


## 단방향 바인딩과 양방향 바인딩에 대한 차이점을 설명

단방향 바인딩 : 데이터 흐름이 한쪽인 경우를 의미한다. 
대표적인 지시어는 v-on, v-bind, {{}} 머스태시 태그
v-on(@) 은 UI에서 데이터 모델(viewModel)을 업데이트 하거나 출력할때 사용한다.
v-bind(:) 는 데이터 모델(viewModel) 에서 업데이트 된 상태를 UI에 반영한다.

양방햔 바인딩 : 데이터 흐름이 양방향이 경우를 의미한다.
대표적인 지시어는 v-model
데이터모델(viewModel)이 변경되면, 자동으로 UI도 변경이 된다.

## 양방향 바인딩 어떻게 생성하나요?

- v-model 지시어를 사용

## 컴포넌트 props 란?

- props 는 상위컴포넌트에서 하위컴포넌트에게 데이터를 전달할때 사용하는 옵션
- vue 에 데이터 흐름은 위에서 아래로 흐르기때문에 하위 컴포넌트가 상위 컴포넌트 상태를 직접 참조할 수 없음
- props 로 상태가 전달이 되면 해당 컴포넌트에 속성이 된다

```vue
Vue.component('child', {
  // props 정의
  props: ['message'],
  // 데이터와 마찬가지로 prop은 템플릿 내부에서 사용할 수 있으며
  // vm의 this.message로 사용할 수 있습니다.
  template: '<span>{{ message }}</span>'
});

```

<child message="안녕하세요!"></child>

## vue 프로젝트를 어떻게 배포하나요?

- SFC(Single File Component) 방식으로 코드를 작성했다면 웹팩 빌드 후, 빌드 결과물을 정적 서버에 올린다. 
- express-static 같은걸로 빌드 후, 서버 올리면 될듯..?

## 컴포넌트란 무엇인가?

- vue component 는 재사용 및 확장성을 위해 코드를 캡슐화한거다.
- vue component 는 vue instance 이기도 하여, 옵션 객체 사용이 가능(root component 에서만 사용하는 옵션 제외)

## filter 란 무엇인가?

- 일반적인 text 형식(format)을 가공해주는 역할을 한다.
- 머스태시 태그와 v-bind 에서 사용 가능하며, | (파이프) 기호와 함께 사용한다.
- 필터 체이닝도 가능하다 ( {{ message | filterA | filterB }}

<!-- in mustaches --> 
{{ message | capitalize }} //  capitalize -> filter

<!-- in v-bind --> 
<div v-bind:id="rawId | formatId"></div> //  formatId -> filter

## 다른 페이지로 리다이렉트(redirect) 어떻게 하나요?
re(다시) + 지시하다(direct) : 다시 지시하는 것

- vue-router 모듈을 이용하여 routing 기능을 구현할 수 있다.
(라우팅이란 출발지부터 목적지까지의 경로를 설정하는것을 의미한다.)
- $router.push();

## vue 앱 구조에 대한 기본 개념 설명

- vue 는 루트 컴포넌트(root instance)를 생성하고 루트 컴포넌트가 최상위를 기준으로 자식컴포넌트들이 tree 구조로 구성됩니다.

```
root component
  ㄴ header component
  ㄴ body component
    ㄴ main component
  ㄴ footer component
```
  
## Vuex 란 무엇인가요?

- vue 앱에 상태관리를 위한 라이브러리
- 모든 컴포넌트에 대한 상태를 중앙집중식으로 관리하는 저장소 역할을 한다.


## vue 에서 mixin 이 필요한 이유는?

- mixin 은 여러 컴포넌트간의 공통으로 사용하고 있는 로직, 상태들을 재사용하는 방법
- 2개의 컴포넌트가 동일한 기능을 가지고 있다고 생각해보자. 만약 같은 메서드를 2개 작성한다면 코드 중복 + 해당 메서드들이 바뀌면 코드를 2번 수정해야한다. -> 이걸 우아하게 mixin 으로 해결 가능하다.
- mixins : []  속성으로 지정하면 된다.
- mixin과 컴포넌트의 옵션이 중첩이 된다면, 두 옵션은 'Merged' 된다.

- 라이프사이클도 믹스인에 정의가 가능하지만, 라이프사이클 함수는 모두 실행된다(mixin -> component)

## AOT와 JIT에 대해 설명해주세요.
JIT는 Just In Time Compile의 약자로 브라우저에서 템프릿 컴파일을 진행하기 때문에 느리다. 또한 JIT 컴파일러를 포함해야하기 때문에 용량도 크다.

AOT는 Ahead Of Time Compile의 약자로 빌드 시 템플릿을 먼저 컴파일을 해둔다. 빌드에는 시간이 더 소요되지만 브라우저에서는 컴파일이 실행되지 않기 때문에 꽤나 빠르다.

그래서 개발 시에는 JIT 방식으로 빠르게 빌드해서 변경사항을 확인하고, 실제 서비스 배포시에는 AOT방식으로 빌드해서 전체 용량 감소 및 컴파일 시간을 없애야한다.

## Vue.js의 computed와 method의 차이를 설명해라
 결과는 같지만 동작방식이 다르다. computed는 계산된 값을 캐시에 저장해뒀다가 값이 변경되면 다시 캐시된 값을 가지고 다시 계산을 한다. 같은 페이지 내의 같은 연산을 수행할 때 효율적이다. 반면 method는 호출될 때 마다 함수를 다시 계산한다.

## computed를 사용해본적이 있나?
댓글 수 제한을 둘 때 사용했다. 댓글 수를 변수로 두고 해당 변수의 사이즈가 3000자 이상이 넘어가면 3000자까지 문자를 splice를 이용하여 자르고 alert창을 띄우는데 사용했다.

## Vue.js의 라이프사이클을 설명해보아라
Creation, Mounting, Updating, Destruction

Creation은 라이프사이클 중 가장 먼저 실행되는 단계이다. 이 단계의 훅에서는 DOM트리에 해당 컴포넌트가 반영이 안되므로 태그의 id나 class에 접근할 수 없다.
훅으로는 beforeCreated, created가 있는데 beforeCreated에서는 data나 event에 접근할 수 없다.

Mounting은 DOM 삽입 단계로 렌더링 되기 직전의 컴포넌트에 접근할 수 있다. 훅으로는 beforeMount, mounted가 있는데 beforeMount훅은 템플릿과 렌더 함수들이 컴파일이 되고 렌더링이되기 직전 단계에 호출이 된다. 아직 까지 DOM element에 직접적으로 접근할 수가 없다. mounted 훅에서, 컴포넌트가 렌더링이 된 상태일 때 호출된다. DOM에 접근할 수 있지만 주의해야할 점은 자식 컴포넌트에서 마운트된 상태임을 보장할 수 없다는 점이다.

Updating은 웹페이지의 내용이나 무언가 바껴서 재렌더링을 해야할 때 실행된다. 훅으로는 beforeUpdate와 updated가 있고 beforeUpdate 훅은 DOM변경이 완료가 되고 패치가 되기 직전에 호출이된다. updated 훅은 재 렌더링이 완료된 이후에 호출이 된다. updated는 패치 이후에 호출되는 훅이라 변화가 끝난 DOM에 접근이 가능하다.

Destruction은 컴포넌트가 해체?파괴될 때 실행된다. 훅으로는 beforeDestroy, destroyed 단계로 beforeDestroy는 해체 직전에 호출되며 모든 DOM과 이벤트들이 남아있다. destroyed는 해체가 완전히 된 후에 호출이되는 훅이다.

## 가상DOM을 설명해주세요.
 가상돔은 추상화한 돔이다. 만약 가상돔을 사용하지 않고 div 태그 1000개에 css 효과가 추가된다고 가정을 한다면 이 천개의 돔노드들을 일일이 검색하고 업데이트를 해줘야한다. 이러한 탐색비용과 업데이트 비용을 좀 더 줄이고자 추상화한 돔에서 탐색과 업데이트를 한 후 변경사항을 실제 돔에 반영한다. 가상돔은 어떻게 돔을 추상화할 것인지, 언제 돔에 변경사항을 적용시킬지에 대한 알고리즘이 핵심이다.






### References
- https://www.fullstack.cafe/blog/20-top-vue-js-interview-questions-2018-updated
- https://velog.io/@katanazero86/vue.js-%EA%B8%B0%EC%88%A0%EB%A9%B4%EC%A0%91-%EC%A7%88%EB%AC%B8%EB%AA%A9%EB%A1%9D
- https://kadamon.tistory.com/23
