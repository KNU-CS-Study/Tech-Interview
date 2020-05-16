# Isolation Level

트랜잭션의 ACID중 Isolation과 관계가 있다

Isolation level이란 특정 트랜잭션이 다른 트랜잭션에서 변경하거나 조회하는 데이터를 볼 수 있도록 허용할지 말지를 결정하는 것



## 격리성 관련 문제점

### (1) Dirty Read

한 트랜잭션(T1)이 데이타에 접근하여 값을 'A'에서 'B'로 변경했고 아직 커밋을 하지 않았을때, 다른 트랜잭션(T2)이 해당 데이타를 Read 하면?

 T2가 읽은 데이타는 B가 될 것이다. 하지만 T1이 최종 커밋을 하지 않고 종료된다면, T2가 가진 데이타는 꼬이게 된다.

(커밋되지 않는 트랜잭션도 읽어서 생기는 문제)

### (2) Non-Repeatable Read

한 트랜잭션(T1)이 데이타를 **Read** 하고 있다. 이때 다른 트랜잭션(T2)가 데이타에 접근하여 값을 변경 또는, 데이타를 삭제하고 커밋을 때려버리면?

그 후 T1이 다시 해당 데이타를 Read하고자 하면 변경된 데이타 혹은 사라진 데이타를 찾게 된다.

(같은 데이터를 2번 read해도 일관적이지 않다)



### (3) Phantom Read

트랜잭션(T1) 중에 특정 조건으로 데이타를 검색하여 결과를 얻었다. 이때 다른 트랜잭션(T2)가 접근해 해당 조건의 데이타 일부를 삭제 또는 추가 했을때, 아직 끝나지 않은 T1이 다시 한번 해당 조건으로 데이타를 조회 하면 T2에서 추가/삭제된 데이타가 함께 조회/누락 된다. 그리고 T2가 롤백을 하면? 데이타가 꼬인다 (데이터를 두번 이상 읽는 쿼리에서 발생하는 이상현상..?)



## Isolation Level의 4단계

**READ UNCOMMITTED**

- 각 트랜잭션에서의 변경 내용이 `COMMIT`이나 `ROLLBACK` 여부에 상관 없이 다른 트랜잭션에서 값을 읽을 수 있다.
- 정합성에 문제가 많은 격리 수준이기 때문에 사용하지 않는 것을 권장한다.
- 아래의 그림과 같이 `Commit`이 되지 않는 상태지만 `Update`된 값을 다른 트랜잭션에서 읽을 수 있다.
- 발생 가능 문제 : Dirty Read, Non-Repeatable Read, Phantom Read

**READ COMMITTED**

- RDB에서 대부분 기본적으로 사용되고 있는 격리 수준이다.
- Dirty Read와 같은 현상은 발생하지 않는다.
- 실제 테이블 값을 가져오는 것이 아니라 Undo 영역에 백업된 레코드에서 값을 가져온다.
- 발생 가능 문제 : Non-Repeatable Read, Phantom Read

#### REPEATABLE READ

- MySQL에서는 트랜잭션마다 트랜잭션 ID를 부여하여 트랜잭션 ID보다 작은 트랜잭션 번호에서 변경한 것만 읽게 된다.
- Undo 공간에 백업해두고 실제 레코드 값을 변경한다.
  - 백업된 데이터는 불필요하다고 판단하는 시점에 주기적으로 삭제한다.
  - Undo에 백업된 레코드가 많아지면 MySQL 서버의 처리 성능이 떨어질 수 있다.
- 이러한 변경방식은 [MVCC(Multi Version Concurrency Control)](https://en.wikipedia.org/wiki/Multiversion_concurrency_control)라고 부른다.

repeatable read -> PHANTOM READ

- 다른 트랜잭션에서 수행한 변경 작업에 의해 레코드가 보였다가 안 보였다가 하는 현상

- 이를 방지하기 위해서는 쓰기 잠금을 걸어야 한다.

- 발생 가능 문제 : Phantom Read

  

#### SERIALIZABLE

- 가장 단순한 격리 수준이지만 가장 엄격한 격리 수준

- 성능 측면에서는 동시 처리성능이 가장 낮다.

- `SERIALIZABLE`에서는 `PHANTOM READ`가 발생하지 않는다.하지만.. 데이터베이스에서 거의 사용되지 않는다.



## Reference

https://feco.tistory.com/45