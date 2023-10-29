# CS Study
![](https://github.com/dev-team-study/cs-study/assets/49775540/2ce09b37-0dd6-4366-98fc-531372e1cab7)
> 기술 면접 대비를 위한 CS 스터디를 진행합니다.
<br>

## 👾 스터디 멤버

|                     [황창현](https://github.com/Hchanghyeon)                     |                      [이현호](https://github.com/charlesuu)                      |                       [소재훈](https://github.com/jay-so)                        |                     [김범석](https://github.com/BeomSeogKim)                        |
|:-----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| <img src="https://avatars.githubusercontent.com/u/92444744?v=4" width="150">  | <img src="https://avatars.githubusercontent.com/u/76809524?v=4" width="150">  | <img src="https://avatars.githubusercontent.com/u/52352476?v=4" width="150">  | <img src="https://avatars.githubusercontent.com/u/110332047?v=4" width="150">  |

<br>

## ⛳ 스터디 진행 방식

| 항목             | 내용                                                         |
| ---------------- | ------------------------------------------------------------ |
| **기간**         | 2023년 10월 11일 ~                                           |
| **장소**         | 온라인 게더타운, 오프라인 강남역                             |
| **요일 및 시간** | 매주 월요일, 수요일 오전 10:00 ~ 12:00 (약 2시간)            |
| **방식**         | 각 CS 과목의 키워드에 해당하는 지식을 학습하고, 자주 나오는 면접 질문의 답변을 정리한다.<br />매 스터디 마다 면접자 2명을 무작위로 뽑고, 나머지 4명이 면접관이 되어 모의 면접을 진행한다.<br />무단으로 불참하거나, 스터디 시작 전까지 PR을 업로드하지 않을 경우 벌금 3,000원을 납부한다.<br />한 달에 3회 이상 무단 불참 시, 스터디에서 퇴장 당할 수 있다. |

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