- Spring 기본
   - Spring vs Spring MVC vs Spring Boot
      - MVC1 vs MVC2
   - dispatcher servlet
   - IoC
   - DI
   - Bean, Component
      - `@Component` `@Service` `@Controller`
      - 생성주기
      - 프로토타입 빈
   - Container
   - VO vs DTO vs DAO
- Spring 심화
   - AOP
      - Spring AOP 어노테이션
      - JDK Dynamic Proxy
      - CGLIB
   - interceptor 
      - filter와 차이점
   - Spring 전체 동작과정

## 질문
### 혁준
1. 후보 없이 특정 기능을 하는 클래스가 딱 1개라면, 구체 클래스를 사용해도 되지 않을까요? 근데, 왜 Spring에선 Bean을 사용 할까요?
2. 생성자 주입 방식을 사용하는 이유가 있나요?
3. default scope 가 어떤 scope인지 이유와 함께 설명하세요.
4. 인스턴스를 새로 만들지 않고 재사용하는 것은 어떤 장점이 있나요?
5. prototype scope 는 어떨 때 사용하는 지 아시나요?
6. 스프링 컨테이너란 무엇인가요?
7. Spring에서 @Controller 와 @RestController 은 어떤 차이가 있나요?
8. 그렇다면, @Controller 로 작성했을 땐 Rest 방식인 String JSON 으로 반환하지 못하나요?
9. @Component 을 메서드 레벨에 선언할 수 있을까? 혹은 @Bean 을 클래스 레벨에 선언할 수 있을까?
10. BeanFactory vs ApplicationContext 차이에 대해 설명해주세요.
11. AOP와 필터, 인터셉터의 차이점에 대해 자세하게 설명해보세요.
12. AOP 를 실제로 사용해 본 경험이 있나요?
13. AOP 동작원리에 대해 설명해보세요.
14. AOP 를 동작시키기 위해 어떤 조건 혹은 어떤 코드를 구성을 해야 AOP 가 정상적으로 동작하는지 아시나요?
15. AOP 적용할 수 있는 포인트가 메서드라고 했을 때 메서드의 시작과 끝에 AOP 를 걸 수가 있습니다. 이때, 메서드를 호출하는 과정에서 메서드가 다른 외부에서의 호출이거나 동일한 클래스 내부에서의 호출이 될 수도 있습니다. 이런 경우에 모두 AOP가 동작하나요? 근거와 함께 설명해주세요.
16. 동적 프록시(JDK Dynamic Proxy)에 대해 설명해주세요.
17. CGLIB(Code Generation Library)에 대해 설명해주세요.
18. VO, DTO 차이에 대해 설명하세요.
19. 엔티티, VO 차이에 대해 설명하세요.
20. DAO(Data Access Object)란 무엇인가요?


### 창현
1. IoC가 무엇이고, IoC Container에 대해서 설명해주세요. 그리고 IoC Container라 불리는 빈 팩토리와 애플리케이션 컨텍스트에 대해서도 말씀해주세요.
2. DI를 진행할 때 `@Autowired`를 사용하게 되는데, 어떤식으로 의존 관계를 주입하는지 아시는 대로 설명해주세요.
3. `@Bean`과 `@Component`의 차이에 대해서 설명해주세요.
4. DAO와 Repository의 차이점에 대해서 알고 꼐신가요?
5. 스프링 프레임워크에서 Bean을 등록할 때는 Proxy로 생성될까요? 일반 Bean으로 생성될까요?
6. JDK Dynamic Proxy와 CGLIB에 대해서 설명해주세요.
7. 필터와 인터셉터의 차이에 대해서 설명해주세요.
8. 필터가 스프링 빈 등록과 주입이 가능할까요?

### 재현
1. 왜 생성자 주입을 사용하나요?
2. 어떻게 Bean을 싱글톤으로 보장할 수 잇는지?
3. 의도적으로 싱글톤을 보장하고 싶지 않을 경우에 할 수 있는 설정?
4. bean을 수동등록하는 이유
5. SpringBootApplication run 이 일어나면 동작하는 과정에 대해 설명해주세요
6. spring동작과정중 refresh 동작 과정에 대해 알고 있나요?
7. ApplicationContext의 정의
8. xml 설정보다 자바 설정이 좋은 이유
9. SpringBoot에서 에러가 발생했을때 동작과정
10. @ControllerAdvice, @RestControllerAdvice 예외처리 동작
11. DynamicProxy와 CGLIB에 대해 IoC컨테이너와 연관지어 설명해주세요
12. AOP에 대해 설명해주세요 프로젝트는 AOP를 어디서 쓰고 있나요? 
13. Autowired의 동작과정에 대해 알고있나요?
14. @Value 의 동작과정이 어떻게 이루어지는 지 알고있나요? 혹은 그 어노테이션에 대해 설명해주세요
15. Bean에 등록되는 키와 value값은 무엇일까용? 프록시일때는?
16. 프록시가 스프링 싱글톤 빈에서 동시성 처리에 용이한 이유는?
17. Bean후처리기에서 프록시로 등록될지, 원본 객체로 등록될지 판단하는 기준

### 범석
- IOC는 무엇인가요?
- Spring에서는 어떻게 IOC를 지원하는지?
- DI가 무엇인지 설명해주시고, DI를 할 수 있는 방법에 대해서 설명해주세요.
- Bean과 Component의 차이에 대해서 설명해주세요
- VO, DTO, DAO의 차이에 대해서 설명해주세요
- AOP란 무엇인지, 주된 용어는 어떤 것이 있는지 설명해주세요.
- JDK DynamicProxy CGLIB는 어떠한 차이점이 존재하는 지 설명해주세요
- Interceptor와 filter의 차이점에 대해서 설명해주세요.

### 현호
1. IoC에 대해 설명해주세요.
2. 다양한 DI 방법과 그 차이점에 대해 설명해주세요.
3. 스프링 빈의 생명주기에 대해 설명해주세요.
4. @Bean과 @Component의 차이점은 무엇인가요?
