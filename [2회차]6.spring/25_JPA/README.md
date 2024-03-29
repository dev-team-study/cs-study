- JPA
   - JDBC, Spring JDBC
   - Sql Mapper(MyBatis), ORM
   - @Transactional
   - JPA, Hibernate
   - 영속성 컨텍스트
   - 즉시/지연 로딩
   - 프록시

## 사전 질문
### 혁준
1. JPA와 MyBatis 차이를 자세하게 설명해주세요.
2. SQL 중심적인 개발의 문제점에 대해 설명하세요.
3. JPA ORM을 왜 사용해야 할까요?
4. 영속성은 정말 성능 향상에 큰 도움이 되나요?
5. 영속성 컨텍스트의 이점 5가지를 설명해주세요.
6. 엔티티 생명주기를 설명해주세요.
7. @Transactional(readonly=true)는 어떤 기능인가요?
8. 읽기에 트랜잭션을 걸 필요가 있을까요? @Transactional 어노테이션을 안 붙이면 되지 않을까요?
9. JPA Propagation 전파 단계를 설명해주세요.
10. OSIV에 대해 설명해주세요
11. 영속성 전이에 대해 설명해주세요.
12. 고아 객체에 대해 설명해주세요.
13. N + 1 문제 무엇인지 원인과 해결방안을 함께 설명해주세요.

### 범석
- JDBC와 Spring JDBC는 어떠한 차이점이 존재하나요?
- Sql Mapper와 ORM의 차이에 대해서 설명해주세요 
- 트랜잭션을 설정하는 방식에는 두가지가 존재하는데 아시는 부분에 대해서 설명해주세요
- @Transactional 어노테이션은 어떤 역할을 하나요?
- @Transactional 어노테이션이 붙은 메서드를 호출했을 때 동작하는 과정에 대해서 설명해주세요 
- 즉시로딩과 지연로딩은 어떤 차이를 지니나요? 
- JPA에서 프록시 객체는 무엇인가요? 
- 고아객체란 무엇인가요?

### 창현
1. 현업에서는 JPA를 많이 사용하기도하지만 JdbcTemplate을 많이 사용하기도 합니다. 그 이유는 무엇인 것 같나요?
2. 객체와 테이블 간의 패러다임 불일치에 대해서 설명해주세요.
3. @Transactional(readOnly=true)가 무엇인지 설명해주세요.
4. JPQL을 사용하게 되면 기존 영속성 컨텍스트의 데이터는 갱신되나요?
5. 즉시 로딩과 지연로딩에 대해서 설명해주세요.
6. JPA에서 사용되는 프록시가 어떻게 사용되고 작동되는지 아는대로 설명해주세요.
7. JPA에서 ID를 조회할 때는 프록시가 초기화 될까요 안될까요?

## 면접 중 질문
### 범석
- ORM은 쿼리를 생성해주는데, 이와 관련해서 단점이 존재하는지?
- 선언적인 부분 외적으로 작용시킬 수 있는 방법이 있는지? 
- @Transactional의 전반적인 동작과정에 대해서 설명해주세요 
- Proxy 객체를 조회하기 위한 조건은 무엇인지? (영속성 컨텍스트 관련 질문)

### 혁준
1. JDBC 설명 및 이점 말하기
2. JDBC를 사용하다가 데이터베이스를 변경해야 할 때 JDBC 코드도 변경되는지?
3. 그렇다면 SQL 중심적인 개발의 문제점은?
4. 현업에서 아직까지도 JPA 대신 JDBCTemplate, MyBatis를 사용하는 경우가 있는데 그 이유가 무엇일까요?
5. 그렇다면, DTO로 변환할 때 편하다고 했는데 JPA에는 DTO 자체를 반환하는 방법이 있을까요?
6. 영속성 컨텍스트 이점 5가지 설명
7. 그럼 정말 이게 성능향상에 도움이 되나요?
8. 플러시 설명 및 플러시 발생 시 일어나는 일 설명
9. 읽기 기능만 한다면 트랜잭션 어노테이션을 붙일 필요가 있을까요? 안붙이면 안되나요?
10. 안붙여도 된다고 했는데, 다른 곳에서 조회할 데이터 수정이 일어나면 어떻게 될까요?
