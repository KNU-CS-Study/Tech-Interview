# IP주소와 DNS

## IP주소

IP주소란 네트워킹이 가능한 장비를 식별하는 주소.



## IPv4 

* 32 비트 길이의 식별자
* 0.0.0.0 ~ 255.255.255.255 까지의 숫자의 조합으로 이루어져 있다.
* 약 43억개의 서로다른 주소를 부여할 수 있다.
* 전세계 공용

### IP주소의 클래스

> 하나의 IP주소에서 네트워크 영역(Network ID)과 호스트 영역(Host ID)을 나누는 방법이자, 약속.

#### A 클래스

* 처음 8bit(1byte)가 Network ID이며 나머지 24bit(3Byte)가 Host ID 이다. 

#### B 클래스

* 처음 16bit(2byte)가 Network ID이며, 나머지 16bit(2Byte)가 Host ID이다.

#### C 클래스

* 처음 24bit(3byte)가 Network ID이며, 나머지 8bit(1Byte)가 Host ID이다. 

#### D 클래스

* Multicast(한 번의 송신으로 메시지나 정보를 여러 컴퓨터에 동시에 전송하는 것, 즉 그때 이용되는 IP)이다.

#### E 클래스

* 예약된 IP주소들로 미래에 쓰기위해 남겨두었다.



## IPv6

* 등장배경
  * 전세계 공용으로 사용되는 IPv4가 고갈될 문제에 처했기 때문이다. 인터넷 사용자가 많아졌다.
* 기존의 IPv4주소체계를 128비트 크기로 확장한 차세대 인터넷 프로토콜 주소.
  * 주소개수가 ipv4 개수의 네제곱.. 거의 무한대라 보면된다. 1조개 이상이다. (2^128)



## DNS

> DNS 또는 Domain Name System은 사람이 읽을 수 있는 도메인 이름(예: www.amazon.com)을 머신이 읽을 수 있는 IP 주소(예: 192.0.2.44)로 변환

* **Domain Name Service**
* Host의 도메인 이름을 네트워크 주소로 바꾸거나 그 반대의 변환을 수행할 수 있도록 하기위해 개발됨.
* IP 주소와 함께 하나의 쌍을 이루어 호스트를 구분할 수 있는 인자가 도메인 이름이며, 이는 32비트의 숫자로 이루어진 IP주소를 사람이 보다 기억하기 쉽게 문자열로 구성한것.



### DNS의 구성요소

* **도메인 네임 스페이스(Domain Name Space)**
  * DNS는 거대한 분산 네이밍 시스템, 도메인 네임 스페이스는 이러한 DNS가 저장/관리하는 계층적 구조를 의미.
  * 최상위 루트 DNS 서버가 존재하고 그 하위로 인터넷에 연결된 노드가 연속해서 이어진 계층구조.
  * 일반적으로 PD에서 사용하는 디렉토리구조와 유사하다.
* **네임 서버(Name Server)**
  * 영문 도메인을 네 자리의 IP주소로 매핑 시켜주는 서버
* **리졸버(Resolver)**
  * 웹 브라우저와 같은 DNS 클라이언트의 요청을 네임 서버로 전달하고 네임 서버로부터 정보(도메인 이름과 IP주소)를 받아 클라이언트에게 제공하는 기능을 수행한다.



### DNS 서비스 유형

* **신뢰할 수 있는 DNS**
  * **신뢰할 수 있는 DNS** 서비스는 개발자가 퍼블릭 DNS 이름을 관리하는 데 사용하는 업데이트 메커니즘을 제공
* **재귀적 DNS**
  * 대개 클라이언트는 신뢰할 수 있는 DNS 서비스에 직접 쿼리를 수행하지 않습니다.
  * 대신에 **해석기** 또는 **재귀적 DNS** 서비스라고 알려진 다른 유형의 DNS 서비스에 연결하는 경우가 일반적



### DNS 동작원리

<img width="820" alt="image" src="https://user-images.githubusercontent.com/36303777/80864617-c2513c00-8cbe-11ea-81af-b42d53229997.png">

1. 웹 브라우저에 www.naver.com을 입력하면 먼저 Local DNS에게 "www.naver.com" 이라는 호스트 네임에대한 IP주소를 질의하여 Local DNS에 없으면 다른 DNS name 서버 정보를 받는다(Root DNS 정보)
2. Root DNS서버에 "www.naver.com" 을 질의.
3. Root DNS서버로 부터 "com 도메인"을 관리하는 TLD(Top-Level Domain) 이름 서버 정보를 정달받음.
4. TLD에 "www.naver.com" 을 질의.
5. TLD에서 "name.com" 관리하는 DNS정보 전달.
6. "naver.com" 도메인을 관리하는 DNS서버에 "www.naver.com" 호스트네임에 대한 IP주소 질의.
7. Local DNS 서버에게 "www.naver.com" 에대한 IP주소 응답.
8. Local DNS는 www.naver.com에 대한 IP주소를 캐싱하고 IP주소 정보 전달.



* Recursive Query : Local DNS 서버가 여러 DNS 서버를 차례대로 (Root DNS -> com DNS -> naver.com DNS 서버) 질의해서 답을 찾아가는 과정. 

### Reference

* https://m.blog.naver.com/PostView.nhn?blogId=hostinggodo&logNo=220589113088&proxyReferer=https:%2F%2Fwww.google.com%2F
* https://limkydev.tistory.com/168
* https://github.com/qkraudghgh/coding-interview/blob/master/Network/IPAndDNS.md
* https://judo0179.tistory.com/37
* https://ijbgo.tistory.com/27
* https://aws.amazon.com/ko/route53/what-is-dns/
