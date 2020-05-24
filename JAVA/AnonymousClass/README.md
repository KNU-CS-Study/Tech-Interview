# 익명클래스 (Anonymous Class)

## 익명클래스란 무엇인가?

클래스의 선언과 객체의 생성을 동시에 하기 때문에 단 한번만 사용될 수 있고, 오직 하나의 객체만을 생성할 수 있는 일회용 클래스.

* 이름이 없기 때문에 생성자를 가질 수 없다.
* 단 하나의 클래스를 상속받거나 단 하나의 인터페이스만을 구현 할 수 잇다.
* 하나의 클래스로 상속받는 동시에 인터페이스를 구현하거나 둘 이상의 인터페이스를 구현할 수 없다.
* 생성자 다음에 중괄호 열고 닫고가 나오면, 해당 생성자 이름에 해당하는 클래스를 상속받는 이름없는 객체를 만든다는 것을 뜻한다.

~~~java
    //추상클래스 Action 
    public abstract class Action{
        public abstract void exec();
    }

    //추상클래스 Action을 상속받은 클래스 MyAction

    public class MyAction extends Action{
        public void exec(){
            System.out.println("exec");
        }
    }

    //MyAction을 사용하는 클래스 ActionExam 
    public class ActionExam{
        public static void main(String args[]){
            Action action = new MyAction();
            action.exec();
        }
    }

    //MyAction을 사용하지 않고 Action을 상속받는 익명 클래스를 만들어서 사용하도록 수정해 보도록 하겠습니다.
    public class ActionExam{
        public static void main(String args[]){
            Action action = new Action(){
                public void exec(){
                    System.out.println("exec");
                }
            };
            action.exec();
        }
    }
~~~







## 왜 사용하는가?

딱 한번 쓰고 재사용하지 않을 것 같은 자식 클래스를  좀더 편하게 쓰기 위해 나온 문법 입니다.





### Reference

* http://blog.naver.com/PostView.nhn?blogId=j931018&logNo=221142327190&parentCategoryNo=&categoryNo=23&viewDate=&isShowPopularPosts=false&from=postView
* https://mommoo.tistory.com/16
* https://deviscreen.tistory.com/25
* https://programmers.co.kr/learn/courses/5/lessons/243

