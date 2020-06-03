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
