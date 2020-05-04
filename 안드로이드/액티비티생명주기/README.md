# 액티비티 생명주기

액티비티는 다음 그림과 같은 생명주기(LifeCycle)를 가지고 있다. 이 생명주기에 따라 적절한 메소드가 호출되므로 이를 숙지해서 액티비티를 작성해야 한다. 

![img](https://kairo96.gitbooks.io/android/content/pic2/2-4-1-1.jpg)

액티비티 생명주기는 onCreate() -> onStart() -> onResume() -> onPause() -> onStop() -> onDestory()순으로 실행되며, 경우에 따라서 onRestart() 메소드가 호출되기도 한다. 이에 대한 자세한 설명은 다음의 액티비티 생명주기 표를 참고하기 바란다.

**API** 액티비티 생명주기

| 메소드      | 설명                                                         | 다음 메소드                  |
| ----------- | ------------------------------------------------------------ | ---------------------------- |
| onCreate()  | 액티비티가 생성될 때 호출되며 사용자 인터페이스 초기화에 사용됨. | onStart()                    |
| onRestart() | 액티비티가 멈췄다가 다시 시작되기 바로 전에 호출됨.          | onStart()                    |
| onStart()   | 액티비티가 사용자에게 보여지기 바로 직전에 호출됨.           | onResume() 또는 onStop()     |
| onResume()  | 액티비티가 사용자와 상호작용하기 바로 전에 호출됨.           | onPause()                    |
| onPause()   | 다른 액티비티가 보여질 때 호출됨. 데이터 저장, 스레드 중지 등의 처리를 하기에 적당한 메소드. | onResume() 또는 onStop()     |
| onStop()    | 액티비티가 더이상 사용자에게 보여지지 않을 때 호출됨. 메모리가 부족할 경우에는 onStop() 메소드가 호출되지 않을 수도 있음. | onRestart() 또는 onDestroy() |
| onDestroy() | 액티비티가 소멸될 때 호출됨. finish() 메소드가 호출되거나 시스템이 메모리 확보를 위해 액티비티를 제거할 때 호출됨. | 없음                         |

※ onStop(), onDestory()는 호출되지 않을 수도 있음

**TIP & TECH** 사용자가 홈 키를 눌렀는지를 파악하는 방법
Activity 클래스에는 onUserLeaveHint() 메소드가 제공되고 있다. 이 메소드가 바로 사용자가 홈 키를 눌렀을 때, 호출되는 메소드이다. 그러므로 이 메소드를 재정의해서 원하는 코드를 작성하면 된다. 참고로 이 메소드가 호출된 뒤에는 Activity의 onPause() 메소드가 호출된다.

Activity의 onUserInteraction() 메소드는 사용자가 터치패드, 키입력 등으로 상호작용 하는지 알 수 있게 해준다. 어떤 상호작용을 하는지는 모름



## REFERENCES

https://kairo96.gitbooks.io/android/content/ch2.4.1.html