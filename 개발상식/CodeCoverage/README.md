# 코드 커버리지(Code coverage)

소프트웨어 테스트가 성공적으로 수행되었는지를 확인하는 방법.

> https://nesoy.github.io/articles/2018-01/Code-Coverage 블로그를 보고 작성하였습니다. 

## 코드 커버리지란

테스트 수행 결과를 정량적인 수치로 나타내는 방법.

* 소프트웨어의 테스트를 논할때 얼마나 테스트가 충분한가를 나타내는 지표 중 하나.
* 소프트웨어 테스트를 진행 했을 때 코드 자체가 얼마나 실행되었는지 숫자로 볼 수 있다.



### 구문 (Statement Coverage)

* 코드 한 줄이 한번 이상 실행된다면 충족된다.

~~~java
int foo (int x, int y)
{
    int z = 0;
    if ((x > 0) && (y > 0))
    {
        z = x;
    }
    return z;
}
~~~

`foo(1,1)`을 호출하게 되면 `(x>0)`과 `(y>0)` 조건 둘 다 만족하므로 `z=x;`를 실행하여 모든 Line을 실행하게 됩니다. 그러므로 테스트 `foo(1,1)`는 `Statement Coverage`에 만족한다고 할 수 있습니다. 반대로 `foo(0,1)`은 if문 만족하지 못하기 때문에 `Statement Coverage`에 만족한다고 할 수 없습니다.



### 결정 (Decision Coverage)(Branch Coverage)

- 전체적인 결과가 참/거짓이면 충족된다.

```java
int foo (int x, int y)
{
    int z = 0;
    if ((x > 0) && (y > 0))
    {
        z = x;
    }
    return z;
}
```

`foo(1,1)`, `foo(0,1)`은 결정 Coverage에 만족합니다. 첫번 째의 `foo(1,1)`은 if문을 통과하여 `z=x`가 실행됩니다. 하지만 두번 째의 `foo(0,1)`은 `(x>0)`이라는 조건에 만족하지 않기 때문에 `z=x`가 실행되지 않습니다. 그러므로 `foo(1,1)`, `foo(0,1)`을 실행하였을 때 if문 전체 결과가 `참/거짓`을 만족하기 때문입니다.



### 조건 (Condition Coverage)

- 각 내부 조건이 참/거짓을 가지게 되면 충족된다.

```java
int foo (int x, int y)
{
    int z = 0;
    if ((x > 0) && (y > 0))
    {
        z = x;
    }
    return z;
}
```

`foo(1,0)`과 `foo(0,1)`는 조건 Coverage에 만족합니다. `(x>0)`에서 `foo(1,0)`에서 `True`이지만 `foo(0,1)`은 `False`입니다. 반대로 `(y>0)`에서 `foo(1,0)`에서 `False`이지만 `foo(0,1)`은 `True`입니다.

그러므로 if문안의 각각 조건을 `true/false`를 둘 다 수행했기 때문에 `조건 (Condition Coverage)`를 만족합니다.





### Reference

* https://nesoy.github.io/articles/2018-01/Code-Coverage