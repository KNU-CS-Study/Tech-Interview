# 데이터베이스 개론

### DB 사용 이유

1. Query (Schema, DML, SQL) 

   > 정규 표현식을 사용한 검색 기능

2. Integrity (Integrity constraints, Types) 

   > 제약조건을 사용하여, 잘못된 입력에 견딤.

3. Update (DDL) 

   > 레코드 정보를 변경함.

4. Multiple Users (Serializability, Concurrency control) 

   > 다중 사용자일 때, 동기화 문제를 해결

5. Crash (Transactions, Commit, Rollback, Recovery) 

   > atomicity가 보장 되어야 하며, commit과 rollback이 구현되면 좋다.

6. Data Physically Separate (Joins, Keys, Foreign keys, Referential integrity) 

   > 물리적으로 떨어진 데이터들을 합쳐서 새로운 정보를 구성

7. Security (Security, Views) 

   > 접근 가능 영역을 나눈다.

8. Efficiency (Indexes, Query optimization, Database tuning) 

   > 데이터가 커질 때 편집이 느려져서는 안된다

9. New Needs (Data mining, Big Data Analytics, Data warehouses, Database API) 

   > 흥미로운 트렌드를 캐거나 예측

   

### 데이터란?

기록될 수 있고, 묵시적 의미를 갖는 것.



### 데이터 베이스란?

 관련된 데이터들의 집합, 

Database Schema + Data

> Schema란 : 데이터의 논리적 구조
>
> Database Schema : Database 에 저장된 data의 논리적 구조.

여러 사람에 의해 공유되어 사용될 목적으로 통합하여 관리되는 데이터의 집합

자료항목의 중복을 없애고 자료를 구조화하여 저장함으로써 자료 검색과 갱신의 효율을 높임



### 데이터베이스 용어

![DataBase 용어](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=http%3A%2F%2Fcfile9.uf.tistory.com%2Fimage%2F993845445A67253915C638)

* **식별자(identifier) :** 여러개의 집합체를 담고있는 관계형 데이터베이스에서 각각의 구분할 수 있는 논리적인 개념
  * **식별자의 특성**
    * 유일성 : 하나의 릴레이션에서 모든 행은 서로 다른 키 값을 가져야 합니다.
    * 최소성 : 꼭 필요한 최소한의 속성들로만 키를 구성해야 합니다.

* **튜플(Tuple) :** 테이블에서 행을 의미합니다. 같은 말로 레코드(Record) 혹은 로우(Row)라고 하기도 해요. 튜플은 릴레이션에서 같은 값을 가질 수 없습니다. 튜플의 수는 카디날리티(Cardinality) 라고 합니다.

* **어트리뷰트(Attribute):** 테이블에서 열을 의미한다. 같은말로 칼럼(Columm)이라고도 하며 어트리뷰트(Attribute)의 수를 의미하는 단어는 디그리(Degree)라고 합니다.


### DBMS란?

사용자들이 데이터 베이스를 만들고 유지할 수 있게 해주는 소프트웨어 패키지/시스템

![DBMS](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=http%3A%2F%2Fcfile1.uf.tistory.com%2Fimage%2F993AAA345A673E0E2B922D)



#### 대표적인 DBMS 종류 및 장단점

1. Oracle
   1. 오라클에서 만들어 판매중인 상업용 데이터베이스
   2. 다양한 운영체제에 설치 가능
   3. MS_SQl이나 MY_SQL보다 대량의 데이터를 처리하기 좋음
   4. 대기업에서 주로 사용하며 글로벌 DB시장 점유율 1위
   5. 오픈소스가 아닌 비공개 소스로 운영

2. My SQL
   1. MySQL사에서 개발, 현재 오라클에 합병됨
   2. 다양한 운영체제
   3. 오픈소스로 이루어진 무료 프로그램(상업적 사용시 비용)
   4. 가격등의 장점을 앞세워 다수의 중소기업에서 사용 중
3. MS SQL
   1. 마이크로소프트사에서 개발한 상업용 DB
   2. 다른 운영체제도 가능하지만 윈도우즈에 특히 특화
   3. 비공개 소스로 폐쇄적(리눅스버전은 오픈소스)
   4. 중소기업에서 주로 사용

* [DB 점유율 순위](https://db-engines.com/en/ranking)



### 데이터베이스 시스템 이란?

DB + DBMS (+ DB Applications)



### 데이터 베이스 디자인

1. 요구사항 명세화와 분석
2. Conceptual design
3. Logical design
4. Physical design
5. Database application development



### DB의 주요 특징들

1. self-describing 

   * 요약본이 catalog (metadata)이 저장되어 있음.

2. Insulation 

   * program-data independence 

   * 저장소가 변경되어도 프로그램이 변경될 필요는 없음

3. Data abstraction 

   * program-data, program-operation independence 를 허용하는 특성
   * 데이터 모델의 informal definition이 data abstraction의 한 예
   *  저장소의 세부사항을 숨기는 역할을함.  (informal definition이 뭐지?)

   > informal definition이란? 비공식적인 정의?

4. support of multiple views of the data 

   * 데이터에 대해 여러가지 뷰 제공

5. sharing of data and multiuser transaction processing 

   *  Must meet **ACID(Atomicity, consistency, isolation, durability)**
   * **Atomicity(원자성)** : All or nothing property. 전부 수행되거나 전혀 수행되지 않은 것과 동일한 효과를 가져야 한다. 이를 위한 SQL statement는 commit/rollback.
   * **Consistency(일관성)** : 하나의 transaction은 DB를 하나의 consistent state(일관된 상태)에서 또 다른 consistent state로 옮기는 것이어야 한다. 이를 위해 DBMS는 integrity constraints(무결성 제약조건)를 만족시켜야 한다.
   * **Isolation(고립성)** : 여러 트랜잭션들이 동시에 수행되더라도 그들을 차례로 하나씩 수행한 것과 동일한 효과를 가져야 한다. 이를 위해 DBMS는 concurrency control을 제공한다. 대표적 방법이 LOCK이다.
   * **Durability(지속성)** : 하나의 트랜잭션의 수행에 의한 결과는 다른 트랜잭션에 의해 변경되지 않는 한 보존되어야 한다. 이를 위해 DBMS는 backup & recovery를 제공한다.


> 트랜잭션이란 ? 
>
> 데이터베이스의 상태를 변환시키는 하나의 논리적인 기능을 수행하기 위한 작업의 단위 또는 한꺼번에 수행되어야 할 일련의 연산들을 의미한다.

### DB사용의 장점들

1. Controlling redundancy (중복 제어) 

   > 각각의 논리적인 데이터를 오직 한 곳에 저장해야한다 (data normalization, 데이터 정규화)

2. Restricting unauthorized access (비인가 접근 제한)

3. Providing persistent storage for program objects (객체들의 영속적인 저장소 제공)

4. Proving storage structures for efficient query processing

   > 쿼리를 효율적으로 수행하기 위한 자료구조 제공
   
5. 데이터의 일관성과 무결성을 유지 할 수 있다.

6. 데이터의 논리적, 물리적 독립성이 보장된다.

7. 항상 최신의 데이터를 유지한다.

8. 데이터를 통합하여 관리할 수 있다.

9. 데이터를 표준화 할 수 있다.




### DBMS 스키마의 3레벨

1. Internal (physical) schema (at the internal level) 

   > 물리적 저장소 구조와 접근 경로를 명시.
   > 
   > **INDEX**

2. Conceptual (logical) schema (at the conceptual level) 

   > 물리적 저장소의 세부사항을 숨기고, 데이터베이스 구조에 집중함. 
   >
   > conceptual 데이터 모델과, implementation 데이터 모델 사용.
   > 
   > **TABLE**

3. External (view level) schema (at the external level) 

   > 다양한 뷰를 제공하기 위해 사용됨.
   >
   > **VIEW**


### Data Independence (데이터 독립)

1. Logical data independence : 외부 스키마를 바꾸지 않고 컨셉츄얼 스키마를 바꿀 수 있는 능력
2. Physical data independence : 컨셉츄얼 스키마를 바꾸지 않고, 내부 스키마를 바꿀 수 있는 능력



### DBMS Language

1. Data Definition Langauge **(DDL, 데이터 정의 언어)**

   * 관계형 데이터베이스의 구조를 정의함
   * 쌍, 속성, 관계 인덱스 파일 위치 등 데이터베이스 고유의 특성을 포함함
   * 테이블과 같은 데이터 구조를 정의하는데 사용되는 명령어들로 (생성,변경,삭제, 이름변경) 데이터 구조와 관련된 명령어들을 말함.
   * 컨셉츄얼/내부 스키마를 위한 것이고, 두 스키마 사이의 매핑을 위한 것이다.
   * ex) CREATE, ALTER, DROP, RENAME, TRUNCATE

2. Data Manipulation Language **(DML, 데이터 조작 언어)**

   * 데이터베이스 검색, 등록, 삭제, 갱신을 하기 위해 사용하는 데이터베이스 언어

   * 데이터베이스 검색과 업데이트에 사용
   * DML 커맨드(called data sublanguage)가 일반적인 목적의 프로그래밍 언어(host language)에 내장 될 수 있음 // c++ or JAVA
   * ex) SELECT, INSERT, UPDATE, DELETE 

3. Data Control Language **(DCL, 데이터 제어 언어)**
   * 데이터베이스에서 데이터에 대한 액세스를 제어하기 위한 데이터베이스 언어 또한 데이터베이스 언어 요소
   * 박탈, 연결, 권한 부여, 질의, 자료 삽입, 갱신, 삭제 등
   * ex) GRANT, REVOKE
4. Transaction Control Language (TCL, 트랜잭션 제어 언어)
   * 논리적인 작업의 단위를 묶어서 DML에 의해 조작된 결과를 작업단위(트랜잭션) 별로 제어하는 명령어를 말함
   * ex) COMMIT, ROLLBACK, SAVEPOINT

### References

* https://brownbears.tistory.com/180
* https://coding-factory.tistory.com/77
* https://brownbears.tistory.com/180
* https://coding-factory.tistory.com/78
