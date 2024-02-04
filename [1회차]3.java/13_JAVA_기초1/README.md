## 13. JAVA_기초1

- Java 기초
  - 접근제어자
  - 클래스, 객체, 인스턴스 차이
  - Overloading vs Overriding
  - Primitive type vs Reference type
     - Call by Reference vs Call by Value
     - Wrapper Class
  - interface vs abstract class
  - Checked Exception vs UnChecked Exception
  - Reflection & Dynamic Proxy

## 질문
### 범석
- 접근 제어자는 왜 사용하나요? 
- 접근 제어자의 접근 범위에 대해서 설명해주세요
- 클래스와 객체 인스턴스의 차이에 대해서 설명해주세요
- 오버로딩과 오버라이딩은 무엇인가요?
- Call By Reference, Call By Value에 대해서 primitive type, reference type과 엮어서 설명해주세요
- Checked Exception, UnChecked Exception에 대해서 설명해주세요.

### 재현
- jpa에서 기본 생성자의 접근제어자를 protected로 제한하는 이유?
- 클래스 멤버와 인스턴스 멤버를 정의하는 차이점 혹은 기준이 있을까요?
- Overriding을 사용하는 예시가 있을까요?
- Animal penguin = new Penguin();가 있고 상위 클래스의 메소드를 override해서 하위 클래스의 메서드에서 재정의한 경우,
상위 클래스의 메소드가 실행되는지, 하위 클래스의 메소드가 실행되는지 설명해주세요..
- 기본타입의 byte 크기를 알고 있나요??
- 기본 타입과 참조 타입이  jvm 메모리 구조 어디에 저장되는지 설명 부탁드립니다.
- wrapper 클래스를 사용하는 이유에 대해서 설명해주세요
- interface와 abstract 클래스의 공통점에 대해서 설명해주세요
- checkedException과 uncheckedException을 비교해서 설명해주세요
- 예외 처리에 대한 특별한 기준이나 전략이 있다면, 설명해주세요
- Reflection의 정의와, 어떻게 생성하고 사용할 수 있는지 설명해주세요
- 스프링에서 Reflection을 사용해본 경험이 있는지 설명해주세요
- Dynamic proxy에 대해 설명해주세요 가능하다면 동작 과정도 설명해주세요
- 스프링에서 사용하는 proxy 방법에 대해 알고 있는 대로 설명해주세요

### 창현
  1. 어떠한 클래스에서 private으로 설정된 필드가 있을 때 이 것을 해당 클래스안에 별도의 이너 클래스를 만들게 되면 해당 이너 클래스에서는 private 필드를 읽을 수 있는지?
  2. 클래스, 객체, 인스턴스에 대해서 설명해주시고 객체와 인스턴스는 어떠한 차이가 있는지 알려주세요.
  3. 오버라이딩과 오버로딩의 차이점을 말씀해주시고 예시를 들어서 설명해주세요.
  4. Call by Reference와 Call by Value는 어떤 것이고 어떤 차이가 있나요?
  5. Wrapper Class인 Integer를 어떠한 메서드의 매개변수로 넣고 해당 메서드안에서 값을 변경시켰을 때 호출한 클래스 내의 Integer 자료형의 값도 변경되는지? 변경되지 않으면 왜 변경되지 않은지?
  6. Checked Exception과 Unchecked Exception이 무엇인지 설명해주세요.
  7. 리플렉션이 무엇인지 설명해주시고, 언제 사용하면 좋을지 간단한 예를 들어서 설명해주세요.
  8. 다이나믹 프록시가 무엇인지 설명해주세요.


### 현호
1. 자바의 4가지 접근제어자에 대해 설명해주세요. (이어서 질문) protected 접근제어자를 쓴 필드에 대해 다른 패키지의 자식 클래스가 접근할 수 있을까요?
2. 클래스, 객체, 인스턴스의 차이에 대해 설명해주세요.
3. 메서드 오버로딩과 오버라이딩의 차이를 설명하고, 각각 어떤 상황에서 사용되는지 예를 들어 설명해주세요.
4. 두 메서드가 메서드명과 매개변수는 같고 반환 타입만 다른 경우. 이를 메서드 오버로딩이라고 볼 수 있을까요?
5. Wrapper 클래스는 어떤 경우에 사용되며, 왜 필요한지 설명해주세요.
6. Call by Reference와 Call by Value의 차이점에 대해 설명해주세요.
7. 자바는 포인터가 존재하는 언어들과 달리 Call by Reference라는 개념이 없다는 주장이 있습니다. 이렇게 생각하시는 분들은 Call by Reference대신에  Call by Sharing이라는 표현을 쓰시기도 하는데요. 이러한 주장이 어떤 맥락에서 나왔다고 생각하시나요?
8. 어떤 클래스에 추상 메서드가 하나도 존재하지 않아도 그 클래스를 추상 메서드로 정의할 수 있을까요?
9. 자바의 리플렉션(Reflection)에 대해 설명하고, 이를 사용하면 어떤 장점과 단점이 있는지 설명해주세요.