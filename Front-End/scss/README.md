# SCSS, SASS

## CSS Preprocessor

HTML, CSS를 다루다보면 Sass, Less, Stylus 등을 볼 수 있다. 이런 애들을 CSS 전(예비)처리기나 `CSS Preprocessor` 라고 부릅니다.

한글로 해석하면 CSS 전처리기라고 하는데 말이 너무 어렵습니다.

쉽게, CSS가 동작을 하기전에 사용하는 기능입니다.

리액트를 하면서 주로 사용하는 CSS 전처리기는

- Sass/SCSS
- postCSS
- Less
- Stylus

여기서 핵심은 Sass와 SCSS를 배워보겠습니다.

## Sass

sass는 css의 전처리기, 즉 해석되어 css로 컴파일되는 스크립트 언어이다.

**Sass는 CSS의 확장**. 궁극적인 목표는 CSS의 결함을 보정하는 것입니다. Sass는 단지 CSS의 부족한 부분만 돕기를 원합니다.

기존 우리가 사용하던 sass에서 많이들 들어봤을 mixin, function 등 여러 기능을 제공한다.

또한 변수 정의를 허용하는데, 변수는 \$ 기호로 시작되고, 변수 할당은 콜론(:)으로 마무리한다.

sassScript는 4가지 자료형을 지원하는데, 수(int), 문자열(string), 컬러, 불린(boolean)을 지원한다.

## SCSS란?

scss는 sass의 3버전에서 등장한 언어이다. 퍼블리셔에게 익숙한 css와 비슷한 구문을 가지고 있으며,

css와 완전히 호환되도록 새로운 구문을 도입한 css의 상위 호환 스타일시트이다.

sass기능을 지원하되, css와 거의 같은 문법으로 사용된다는 점에서, 퍼블리셔들에게 각광받는 언어이다.

### Sass와 SCSS의 차이점

```
Sass는 처음에 들여쓰기의 감지를 그 핵심 특성으로 갖는 구문을 가리켰습니다.

얼마 지나지 않아, Sass를 유지하는 사람들은 Sassy CSS를 의미하는 SCSS라는 CSS 친화적인 구문을 제공함으로써 Sass와 CSS 사이의 차이를 좁히기로 결정했습니다.

모토는 이렇습니다: 만약 유효한 CSS라면, 유효한 SCSS이다.

그 이후로, Sass(전처리기)는 두 가지 다른 구문을 제공해 오고 있습니다: 들여쓰기 구문으로도 알려진 Sass(전부 대문자가 아닙니다, 제발), 그리고 SCSS.

둘은 정확히 동등한 기능을 갖고 있기 때문에 어느 것을 사용할지는 여러분에게 달렸습니다. 지금 시점에서는 이것은 순전히 미관상의 문제입니다.
```

#### [sass의 문법]

```scss
ul.list
	overflow:hidden
	li
    	float:left
        width:200px
        padding: 20px 30px
```

#### [scss의 문법]

```scss
ul.list {
  overflow: hidden;
  li {
    float: left;
    width: 200px;
    padding: 20px 30px;
  }
}
```

큰차이는 없고 미관상의 차이라는 Sass와 SCSS라는 내용이 핵심인것 같습니다. sass의 경우 '들여쓰기'로 구분하고, scss는 기존 css와 같이 { }로 범위를 구분한다.

가독성을 따져보자면 sass가 더 깔끔하고 간단하지만,

깔끔하고 간단한 sass를 선호하는 사람이 있는 반면, 기존 css 문법과 비슷한 scss를 선호하는 사람도 많다.

### References

- https://nm817.tistory.com/39
- https://sheldhe93.tistory.com/4
- https://heropy.blog/2018/01/31/sass/
