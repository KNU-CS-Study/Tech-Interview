## Q1. Vue.js 가 뭔가요?
- Even You(에번 유) 가 2014년도에 발표한 자바스크립트 프레임워크
- 동적인 사용자 인터페이스(UI) 를 만들기 위한 프레임워크

## Q2. Vue instance 는 어떻게 생성하나요?
- Vue() 생성자 함수를 이용하여 생성
- 생성시 옵션 객체를 전달
let vm = new Vue({});
- vue component 도 vue instance 와 동일하다.


## Q3. 단방향 바인딩과 양방향 바인딩에 대한 차이점을 설명

단방향 바인딩 : 데이터 흐름이 한쪽인 경우를 의미한다. 
대표적인 지시어는 v-on, v-bind, {{}} 머스태시 태그
v-on(@) 은 UI에서 데이터 모델(viewModel)을 업데이트 하거나 출력할때 사용한다.
v-bind(:) 는 데이터 모델(viewModel) 에서 업데이트 된 상태를 UI에 반영한다.

양방햔 바인딩 : 데이터 흐름이 양방향이 경우를 의미한다.
대표적인 지시어는 v-model
데이터모델(viewModel)이 변경되면, 자동으로 UI도 변경이 된다.

## Q4. 양방향 바인딩 어떻게 생성하나요?

- v-model 지시어를 사용

## Q5. 컴포넌트 props 란?

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

## Q6. vue 프로젝트를 어떻게 배포하나요?

- SFC(Single File Component) 방식으로 코드를 작성했다면 웹팩 빌드 후, 빌드 결과물을 정적 서버에 올린다. 
- express-static 같은걸로 빌드 후, 서버 올리면 될듯..?

## Q7. 컴포넌트란 무엇인가?

- vue component 는 재사용 및 확장성을 위해 코드를 캡슐화한거다.
- vue component 는 vue instance 이기도 하여, 옵션 객체 사용이 가능(root component 에서만 사용하는 옵션 제외)

## Q8. filter 란 무엇인가?

- 일반적인 text 형식(format)을 가공해주는 역할을 한다.
- 머스태시 태그와 v-bind 에서 사용 가능하며, | (파이프) 기호와 함께 사용한다.
- 필터 체이닝도 가능하다 ( {{ message | filterA | filterB }}

<!-- in mustaches --> 
{{ message | capitalize }} //  capitalize -> filter

<!-- in v-bind --> 
<div v-bind:id="rawId | formatId"></div> //  formatId -> filter

## Q9. 다른 페이지로 리다이렉트(redirect) 어떻게 하나요?
re(다시) + 지시하다(direct) : 다시 지시하는 것

- vue-router 모듈을 이용하여 routing 기능을 구현할 수 있다.
(라우팅이란 출발지부터 목적지까지의 경로를 설정하는것을 의미한다.)
- $router.push();

## Q10. vue 앱 구조에 대한 기본 개념 설명

- vue 는 루트 컴포넌트(root instance)를 생성하고 루트 컴포넌트가 최상위를 기준으로 자식컴포넌트들이 tree 구조로 구성됩니다.

```
root component
  ㄴ header component
  ㄴ body component
    ㄴ main component
  ㄴ footer component
```
  
## Q11. Vuex 란 무엇인가요?

- vue 앱에 상태관리를 위한 라이브러리
- 모든 컴포넌트에 대한 상태를 중앙집중식으로 관리하는 저장소 역할을 한다.


## Q12. vue 에서 mixin 이 필요한 이유는?

- mixin 은 여러 컴포넌트간의 공통으로 사용하고 있는 로직, 상태들을 재사용하는 방법
- 2개의 컴포넌트가 동일한 기능을 가지고 있다고 생각해보자. 만약 같은 메서드를 2개 작성한다면 코드 중복 + 해당 메서드들이 바뀌면 코드를 2번 수정해야한다. -> 이걸 우아하게 mixin 으로 해결 가능하다.
- mixins : []  속성으로 지정하면 된다.
- mixin과 컴포넌트의 옵션이 중첩이 된다면, 두 옵션은 'Merged' 된다.

- 라이프사이클도 믹스인에 정의가 가능하지만, 라이프사이클 함수는 모두 실행된다(mixin -> component)

### References
- https://www.fullstack.cafe/blog/20-top-vue-js-interview-questions-2018-updated
- https://velog.io/@katanazero86/vue.js-%EA%B8%B0%EC%88%A0%EB%A9%B4%EC%A0%91-%EC%A7%88%EB%AC%B8%EB%AA%A9%EB%A1%9D
