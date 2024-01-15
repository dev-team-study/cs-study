- Spring 기본
  - IoC
  - DI
  - Bean, Component
     - @Component @Service @Controller
  - Container
  - VO vs DTO vs DAO
- Spring 심화
  - AOP
    - JDK Dynamic Proxy
    - CGLIB

## 질문
### 창현
- IoC와 DI의 개념에 대해서 설명해주세요.
- IoC Container의 종류로 BeanFactory와 ApplicationContext가 있는 것으로 알고 있는데 이 2가지의 차이점을 알고 계신가요?
- 의존 관계란 무엇일까요?
- DI, 의존 관계 주입의 종류를 아는대로 다 얘기해주세요.
- 빈과 컴포넌트 어노테이션의 차이점에 대해서 알려주세요.
- 컴포넌트와 서비스, 컨트롤러 어노테이션의 차이점에 대해서 알려주세요.
- VO와 DTO, DAO에 대해서 간단하게 설명해주세요.
- VO를 사용해보신적이 있으신지 있다면 어느 상황에서 사용해보셨는지 알려주세요.
- VO를 사용하셨을 때의 이점은 무엇이 있었나요?
- AOP가 무엇인지 설명해주세요.
- Self Invocation에 대해서 아시는게 있다면 말씀해주세요.
- 프록시 패턴에 대해서 설명해주세요.
- JDK Dynamic Proxy에 대해서 설명해주세요.
- CGLIB에 대해서 설명해주세요.
- 위와 같은 JDK Dynamic Proxy나 CGLIB을 직접 이용해서 사용해보신적이 있으신가요? 있다면 언제 사용하셨는지 알려주세요.
### 재현
- 런타임 의존성, 컴파일 의존성 차이
- 생성자 주입의 장점 (@Autowired를 사용하면 안되는 이유)
- 언제 수동 빈을 등록하는가?
- 빈 component, configuration의 차이
- 빈의 정의
- IoC의 역할은 무엇인가요?
- self invocation을 해결하는 방법
- cglib의 한계에 대해 알고계신가요?
- AOP에 대해서 정의 그리고 어떤 것들이 있는지 아는대로 설명해주세요
### 범석
- IOC와 DI의 개념에 대해서 설명해주세요.
- DI 방식에는 어떠한 방식이 존재하는 지 설명해주세요.
- Bean Component는 어떠한 차이점을 지니는지 설명해주세요
- Spring에서 Container는 무엇인가요?
- VO, DTO, DAO 의 역할에 대해서 설명해주세요
- JDK Dynamic Proxy는 무엇인가요
- CGLIB는 무엇인가요
- Spring에서는 JDK Dynamic Proxy, CGLIB를 어떻게 사용하나요? 
### 현호
- IoC와 DI의 개념은 무엇인가요?
- @Bean과 @Component의 차이점은 무엇인가요? 어떤 경우에 사용하나요?
- @Component와 @Service, @Controller, @Repository의 차이점은 무엇인가요?
- IoC컨테이너란 무엇인가요? Bean Factory, Application context의 차이점은 무엇인가요?
- 빈의 Scope에 대해 설명해주세요. 싱글톤과 프로토타입의 차이는 무엇인가요?
- VO, DTO, DAO의 개념과 차이점은 무엇인가요?
- AOP란 무엇인가요? AOP의 장점은 무엇인가요?
- AOP에서 사용되는 용어인 Target, Advice, Join Point, Pointcut, Advisor, Weaving에 대해 설명해주세요.
- 스프링 AOP의 빈 등록 과정은 어떻게 되나요?
- 동적 프록시에 대해 설명해주세요. JDK Dynamic Proxy와 CGLIB의 차이점은 무엇인가요?