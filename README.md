# CS Study
![](https://github.com/dev-team-study/cs-study/assets/49775540/2ce09b37-0dd6-4366-98fc-531372e1cab7)
> 기술 면접 대비를 위한 CS 스터디를 진행합니다.
<br>

## 👾 스터디 멤버

|                     [황창현](https://github.com/Hchanghyeon)                     |                      [이현호](https://github.com/charlesuu)                      |                       [김범석](https://github.com/BeomSeogKim)                        |                       [조재현](https://github.com/HandmadeCloud)                        |
|:-----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| <img src="https://avatars.githubusercontent.com/u/92444744?v=4" width="150">  | <img src="https://avatars.githubusercontent.com/u/76809524?v=4" width="150">|  <img src="https://avatars.githubusercontent.com/u/110332047?v=4" width="150">  | <img src="https://avatars.githubusercontent.com/u/77893164?v=4" width="150">  |

<br>

## ⛳ 스터디 진행 방식

| 항목             | 내용                                                         |
| ---------------- | ------------------------------------------------------------ |
| **기간**         | 2023년 10월 11일 ~                                           |
| **장소**         | 온라인 게더타운, 오프라인 강남역                             |
| **요일 및 시간** | 매주 월요일, 수요일, 금요일 오전 10:00 ~ 11:00 (약 1시간)            |
| **방식**         | 각 CS 과목의 키워드에 해당하는 지식을 학습하고, 자주 나오는 면접 질문의 답변을 정리한다.<br />매 스터디 마다 면접자 2명을 무작위로 뽑고, 나머지 인원이 면접관이 되어 모의 면접을 진행한다.<br />무단으로 불참하거나, 스터디 시작 전까지 PR을 업로드하지 않을 경우 벌금 3,000원을 납부한다.<br />한 달에 3회 이상 무단 불참 시, 스터디에서 퇴장 당할 수 있다. |

<br>

## 📋 각종 컨벤션

### 📁 패키지 구조

```
Cs-study
    ├── database
    |   └── 01_관계형_데이터베이스
    |       ├── README.md => 당일에 나온 모든 질문 아카이빙
    |       ├── 범석.md
    |       ├── 창현.md
    |       └── ...
    ├── network
    |   └── ...
    ...
```



### 📍 커밋 및 PR

1. **커밋 메시지**

   ```
   {과목} {내용} 문서 작성(수정) [이름]
   ```

   - 작성 예시) `DB 01_관계형_데이터베이스 문서 작성 [황창현]`
   - 수정 예시) `DB 01_관계형_데이터베이스 문서 수정 [황창현]`

2. **PR**

   ```
   {과목} {내용} 제출 [이름]
   ```

   - PR 예시) `DB 01_관계형_데이터베이스 제출 [황창현]`

<br>

## 📌 키워드

### 1️⃣ 데이터베이스(DB)

- 관계형 데이터베이스
  - 데이터베이스와 파일시스템의 차이
  - 관계형 데이터베이스의 개념과 장단점
  - DDL, DML, DCL, TCL
  - Key
- MySQL 아키텍처
  - innodb
  - 쿼리동작 방식
- Join
- 이상 현상과 정규화
- 트랜잭션
  - 트랜잭션 개념
  - ACID
  - Commit, Rollback
  - 트랜잭션 격리수준
  - LOCK, 교착상태
- 인덱스
  - 인덱스 개념
  - 인덱스 종류
  - Clustered index, Non-Clustered index
  - 인덱스 자료구조
- Master/Slave
- Sharding
- NoSQL
  - NoSQL의 개념
  - RDB VS NoSQL
  - Redis 동작원리

### 2️⃣ 네트워크 (Network)

- 네트워크 레이어
    - OSI 7계층
    - TCP/IP 4계층
    - IP
        - IPv4 vs IPv6
        - subnet
        - CIDR
- 통신
    - TCP
        - 흐름제어, 혼잡제어, 오류제어
        - 3-way-handshake, 4-way-handshake
    - UDP
    - HTTP
        - HTTP status code
        - HTTP method
        - HTTP 1.1, 2.0, 3.0
    - HTTPS, SSL/TSL
    - DNS
    - 기타 : socket, STOMP, SMTP (프로젝트에서 사용한 경우)
- Web
    - Web Server vs WAS
    - Web Server
        - apache vs nginx (동작원리)
        - SSL offloading
        - reverse proxy
        - load balancing
            - L7 vs L4
            - 알고리즘
    - Web cache
    - URI, URN, URL
    - Rest API
- 보안
    - CORS
    - XSS
    - SQL Injection
- 인증
    - cookie
    - session
    - JWT


### 3️⃣ Java
- 객체지향
   - 4가지 특징
   - 5원칙 (SOLID)
   - 객체지향 vs 절차지향 vs 함수형 프로그래밍
- JDK, JRE, JVM
   - 컴파일 과정
   - 컴파일 언어 vs 인터프리터 언어
   - JVM 메모리 구조
   - Garbage Collector 동작과정
   - Java8의 큰 특징 + Java11과의 차이점
- Java 기초
   - 접근제어자
   - 클래스, 객체, 인스턴스 차이
   - Overloading vs Overriding
   - Primitive type vs Reference type
      - Call by Reference vs Call by Value
      - Wrapper Class
   - interface vs abstract class 
   - Checked Exception vs UnChecked Exception
   - static
   - final
   - generic
   - stream, lambda
   - Reflection & Dynamic Proxy
 - Java 컬렉션
   - hashcode() & equals()
   - Thread Safe & Syncronized
   - String
      - String vs StringBuffer vs StringBuilder 
      - Immutable Object
      - `String a = ""` vs `String a = new String("")`
   - List
      - ArrayList vs LinkedList
   - Map
      - HashTable vs HashMap vs LinkedHashMap vs TreeMap
      - HashMap vs ConcurrentHashMap

### 4️⃣ Spring

- Servlet
   - 개념
   - tomcat
   - filter
   - servlet container
   - 동작과정
- Spring 기본
   - Spring vs Spring MVC vs Spring Boot
      - MVC1 vs MVC2
   - dispatcher servlet
   - IoC
   - DI
   - Bean, Component
      - `@Component` `@Service` `@Controller`
   - Container
   - VO vs DTO vs DAO
- Spring 심화
   - AOP
      - JDK Dynamic Proxy
      - CGLIB
   - interceptor 
      - filter와 차이점
   - Spring 전체 동작과정
- JPA
   - JDBC, Spring JDBC
   - Sql Mapper(MyBatis), ORM
   - JPA, Hibernate
   - 영속성 컨텍스트
   - 즉시/지연 로딩
   - 프록시
   - 고아객체
   - 단뱡향/양방향 매핑
   - N + 1 문제
- 테스트 
   - DDD, TDD
   - Junit4 vs Junit5
   - 단위, 통합, 인수 테스트
   - stub, mock
   - SpringBoot 계층별 테스트 방법
   - 테스트 커버리지 (JACOCO)
