# AJAX

* JavaScript의 라이브러리 중 하나.
* Asynchronous Javascript And Xml(비동기식 자바스크립트와 xml)의 약자.
* JavaScript를 사용한 비동기 통신.
* 클라이언트와 서버간에 XML 데이터를 주고받는 기술.



## Ajax를 사용하는 이유(장점)

* HTTP프로토콜 클라이언트쪽에서 Request를 보내고 Server쪽에서 Response를 받으면 이어졌던 연결이 끊기게 되어 있어서 화면의 내용을 갱신하려면 다시 Request를 하고 Request를 하면서 페이지 전체를 갱신하게 됩니다.
  * 하지만 이렇게 하면 페이지 일부 갱신시에도 전체를 로드해야되서 오버헤드가 큽니다.
* Ajax는 html 페이지 전체가 아닌 일부분만 갱신할 수 있도록 XML HttpRequest객체를 통해서 서버에 request를 합니다. 
* 이 경우 Json이나 xml 형태로 필요한 데이터만 받아 갱신하기 때문에 그만큼의 자원과 시간을 아낄 수 있습니다. 
* 서버에 Data만 전송하면 되므로 전체적인 코딩의 양이 줄어든다.



### Ajax의 단점

* 히스토리 관리가 안된다. 
  * Pjax를 통해 해결가능하다. 그래서 웹 브라우저상에서 페이지 이동이나 뒤로가기 앞으로가기 이력관리를 실제 피이지 이동없이 구현해주는 jQuery의 pushState와 Ajax를 합친 개념.
* 연속으로 데이터를 요청하면 서버 부하가 증가할 수 있다.
* XMLHttpRequest를 통해 통신을 하는 경우 사용자에게 아무런 진행정보가 주어지지 않는다.

> 가장 큰이유는 속도향상. 

### Reference

* https://coding-factory.tistory.com/143

