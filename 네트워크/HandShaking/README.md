# TCP 3-4 Way-Handshake

### TCP 3-way Handshake 란?

TCP는 장치들 사이에 논리적인 접속을 성립(establish)하기 위하여 three-way-handshake를 사용한다.



TCP 3 Way handshake는 TCP/IP  프로토콜을 이용해서 통신을 하는 응용프로그램이 데이터를 전송하기 전에 먼저 정확한 전송을 보장하기 위해 상대방 컴퓨터와 사전에 세션을 수립하는 과정을 의미한다.

```haskell
CLIENT > SERVER : TCP SYN

SERVER > CLIENT : TCP SYN ACK

CLIENT > SERVER TCP ACK
```

**SYN** : 'Synchronize sqeuence numbers'

**ACK** : 'Acknowledgment'



**TCP의 3-way Handshaking 역할**

- 양쪽 모두 데이터를 전송할 준비가 되었다는 것을 보장한다

- 실제로 데이터 전달이 시작하기 전에 **다른 쪽이 준비되었다는 것을 알 수 있도록 한다.**

- 양쪽 모두 상대편에 대한 초기 순차일련번호를 얻을 수 있도록 한다.

![img](https://t1.daumcdn.net/cfile/tistory/225A964D52F1BB6917)

**[STEP 1]**

A클라이언트는 B서버에 접속을 요청하는 SYN 패킷을 보낸다. 이때 A클라이언트는 SYN 을 보내고 SYN/ACK 응답을 기다리는**SYN_SENT 상태**가 되는 것이다.

 

**[STEP 2]** 

B서버는 SYN요청을 받고 A클라이언트에게 요청을 수락한다는 ACK 와 SYN flag 가 설정된 패킷을 발송하고 A가 다시 ACK으로 응답하기를 기다린다. 이때 B서버는 **SYN_RECEIVED 상태**가 된다.

 

**[STEP 3]**

A클라이언트는 B서버에게 ACK을 보내고 이후로부터는 연결이 이루어지고 데이터가 오가게 되는것이다. 이때의 B서버 상태가 **ESTABLISHED** 이다.

위와 같은 방식으로 통신하는것이 신뢰성 있는 연결을 맺어 준다는 TCP의 3 Way handshake 방식이다.



**TCP의 4-way Handshaking**

- 3-Way handshake는 TCP의 연결을 초기화 할 때 사용한다면, 
- 4-Way handshake는 세션을 종료하기 위해 수행되는 절차입니다.

![img](https://t1.daumcdn.net/cfile/tistory/2678E035537EEE9126)



**[STEP 1]**

통신을 종료하고자 하는 Client가 서버에게 FIN 패킷을 보내고 자신은 FIN_WAIT_1 상태로 대기한다.



**[STEP 2]** 

FIN 패킷을 받은 서버는 해당 포트를 CLOSE_WAIT으로 바꾸고 잘 받았다는 ACK 를 Client에게 전하고 ACK를 받은 Client는 상태를 FIN_WAIT_2로 변경한다.

그와 동시에 Server에서는 해당 포트에 연결되어 있는 Application에게 Close()를 요청한다.

 

**[STEP 3]**

Close() 요청을 받은 Application은 종료 프로세스를 진행시켜 최종적으로 close()가 되고 server는 FIN 패킷을 Client에게 전송 후 자신은 LAST_ACK 로 상태를 바꾼다.

 

**[STEP 4]**

FIN_WAIT_2 에서 Server가 연결을 종료했다는 신호를 기다리다가 FIN 을 받으면 받았다는 ACK를 Server에 전송하고 자신은 TIME_WAIT 으로 상태를 바꾼다. (TIME_WAIT 에서 일정 시간이 지나면 CLOSED 되게 된다.)

최종 ACK를 받은 서버는 자신의 포트도 CLOSED로 닫게 된다.



#### TIME_WAIT란?

그런데 만약 "Server에서 FIN을 전송하기 전에 전송한 패킷이 Routing 지연이나 패킷 유실로 인한 재전송 등으로 인해 FIN패킷보다 늦게 도착하는 상황"이 발생한다면 어떻게 될까요? 



Client에서 세션을 종료시킨 후 뒤늦게 도착하는 패킷이 있다면 이 패킷은 Drop되고 데이터는 유실될 것입니다. 

이러한 현상에 대비하여 Client는 Server로부터 FIN을 수신하더라도 일정시간(디폴트 240초) 동안 세션을 남겨놓고 잉여 패킷을 기다리는 과정을 거치게 되는데 이 과정을 **"TIME_WAIT"** 라고 합니다.



### 그 외 비정상 종료

다양한 상황에 따른 연결의 종료를 적절하게 처리하지 못하면, FIN_WAIT_1, FIN_WAIT_2, CLOSE_WAIT 상태로 남아 계속 기다리는 상황이 올 수 있다.



- **CLOSE_WAIT 상태** : 어플리케이션에서 close()를 적절하게 처리해주지 못하면, TCP 포트는 CLOSE_WAIT 상태로 계속 기다리게 된다. 이렇게 CLOSE_WAIT 상태가 statement에 많아지게 되면, Hang 이 걸려 더이상 연결을 하지 못하는 경우가 생기기도 한다. 따라서 어플리케이션 개발시 여러 상황에 따라 close() 처리를 잘 해줘야 한다.



- **FIN_WAIT_1 상태** : FIN_WAIT_1 상태라는 것은 상대방측에 커넥션 종료 요청을 했는데, ACK를 받지 못한 상태로 기다리고 있는 것이다. 이것은 아마 서버를 찾을 수 없는 것으로, 네트워크 및 방화벽의 문제일 수 있다.

 (FIN_WAIT_1 의 상태는 일정 시간이 지나 Time Out이 되면 자동으로 닫는다.)



- **FIN_WAIT_2 상태** : FIN_WAIT_2 상태는 클라이언트가 서버에 종료를 요청한 후 서버에서 요청을 접수했다고 ACK를 받았지만, 서버에서 종료를 완료했다는 FIN 을 받지 못하고 기다리고 있는 상태이다. 이상태는 양방의 두번의 통신이 이루어졌기 때문에 네트워크의 문제는 아닌 것으로 판단되며,(FIN 을 보내는 순간에 순단이 있어 못받은 것일 수도 있다.) 서버측에서 CLOSE를 처리하지 못하는 경우일 수도 있다. FIN_WAIT_2 역시 일정시간 후 Time Out이 되면 스스로 Closed 하게 된다.



- 어떠한 이유에서 FIN_WAIT_1과 FIN_WAIT_2 상태인 연결이 많이 남아있다면, 문제가 발생할 수 있다. 물론 일정 시간이 지나 Time Out이 되면 연결이 자동으로 종료되긴 하지만, 이 Time Out이 길어서 많은 수의 소켓이 늘어만 난다면, 메모리 부족으로 더 이상 소켓을 오픈하지 못하는 경우가 발생한다.

 (이 경우는 네트워크나 방화벽 또는 어플리케이션에서 close() 처리 등에 대한 문제등으로 발생할 수 있으며, 원인을 찾기가 쉽지 않다.)



### **SYN Flooding 공격이란?**

신플루딩공격이란 TCP세션이 연결될 때의 취약성을 이용한 서버공격이다.

먼저 TCP의 기본적인 연결단계는 아래와 같습니다.

- A(소스서버)가 B(목적지서버)에게 접속을 요청하는 SYN패킷을 보낸다.

- B는 요청을 수락한다는 SYN과 ACK패킷을 A에게 보낸다.

- A가 B에게 ACK를 보내면 연결이 이루어지고 본격적이 데이터교환이 이루어진다.

위의 2번단계에서 목적지서버(B)는 소스서버(A)가 ACK패킷을 보내주기를 계속적으로 기다리는 것이 아니라 일정시간 후 요청이 오지 않으면 백로그큐(Backlog Queue)가 허용하는 공간에 연결정보(로그)를 보관하게 됩니다.

이러한 상태가 지속적으로 요청되어 연결정보(로그)가 쌓이게 되면 목적지서버(B)의 특정서비스가 마비될 수 있습니다.

**이러한 공격을 DOS공격의 일종인 SYN Flooding 공격이라고 합니다.**

Syn 로그 기록후 Timeout 까지의 대기 시키는데(Timeout 후에는 로그가 소멸) 그 타임아웃 시점보다 짧게 Syn 요청을 해서 스택을 채워 네트웍을 마비시키기도 하고 Invalid 한 값의 Syn으로 무차별적으로 이루어 지기도 한다.





### REFERENCE

https://mindnet.tistory.com/entry/네트워크-쉽게-이해하기-22편-TCP-3-WayHandshake-4-WayHandshake [Mind Net]

https://skibis.tistory.com/68 [Skibi's Notepad]

https://hyeonstorage.tistory.com/287

