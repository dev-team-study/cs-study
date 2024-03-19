 - Java 기초
   - Checked Exception vs UnChecked Exception
   - static
   - final
   - generic
   - stream, lambda
   - Reflection & Dynamic Proxy
 - Java 컬렉션
   - hashcode() & equals()
   - Thread Safe & Syncronized
     - Volatile
     - AtomicInteger
   - String
      - String vs StringBuffer vs StringBuilder 
      - Immutable Object
      - `String a = ""` vs `String a = new String("")`

# 질문
## 재현
- static은 멀티스레드 환경에서 안전할까요?
- final은 완벽히 불변성을 보장할까요? 내부의 상태 변경을 보장하지는 않는다. (ex arrayList의 add)
- 불변성을 보장받는 방법? 객체의 경우 생성자를 통해 값을 주입받음
- stream의 forEach만 사용하는게 왜 좋지 않을까요?
- 람다 활용의 장단점
- hash충돌에 대해서 설명해주세요
- 자바의 모든 클래스는 Object 클래스를 상속받습니다. 그리고 Object클래스에는 equals() 와 hashCode() 라는 메소드가 선언되어 있습니다. 이 메소드들은 각각 어떤 역할일까요? 이 둘의 차이점은 무엇일까요?
- "hashCode" 를 잘못 오버라이딩하면 "HashMap" 등 hash 콜렉션의 성능이 떨어질 수가 있습니다. 어떤 케이스일 때 그럴 수 있을까요? (일관성 없는 해시코드 반환, 해시충돌 자주 발생, equals를 재정의하지 않는 경우)
- hashmap은 내부적으로 어덯게 구현되어있나요? (내부는 링크드 리스트)
- hashmap의 시간복잡도, 잘못 오버라이딩 한 경우의 시간 복잡도 (O(1) -> key값을 탐색, O(n) linkedList의 조회 시간 복잡도) 
- stringbuilder와 stringbuffer의 차이 : builder는 동기화를 하지 않아 속도가 빠름, buffer는 비동기에 적합해 웹이나 소캣처럼 동작한다.
- 왜 syncrnized키워드가 걸리면 느린지 동작원리와 함께 설명해주세요 lock을 건다. syncronized 키워드가 걸린 모든 object에 대해서 락이 걸린다. 클래스, 인스턴스 단위로락이 걸리기 떄문에 일를 유의해서 사용해야 한다.
- 싱글 스레드로 접근하면 syncronized 적용 여부에 따라 성능이 같을까요 미미하지만 불필요한 오버헤드는 발생할 수도
- List와 비교했을 때 ArrayList만의 타입 특징? 연속적인 자료구조, 데이터 추가시 인덱스를 고려해야 함 indexOutOfBoundsException발생 가능
- arrayList와 배열의 차이점 (배열의 크기는 변경 불가능, 메모리 관리편함, inde를 통한 접근이 빠름) (arrayList 동적 할당, 배열보다 느림)
- 배열로 구현되어있으면 크기 제한 문제가 걸릴텐데. 무한히 데이터를 받을 수 있는지? 정적인 크기, ArrayList의 경우에는 시스템 자원의 한계로 문제가 생길수도
- volatile는 가시성을 보장해준다고 하는데, 가시성에 대해 설명해주세요<br>
 
가시성 : 하나의 스레드에서 변경된 변수의 값을 다른 스레드에서 즉시 알수 있어야 한다. 하나의 스레드는 작업 이후 캐시를 사용하고 그 캐스를 읽어 사용하기때문에 메인 메모리와 동기화되지 않은 캐시 값을 읽을 수 있다. <br>
volatile는 메인 메모리에 직접 접근해 변수 값이 변경되면 모든 스레드에게 변경된 값을 즉시 보장한다. 하지만 원자적 연산이나 스레드 상호 배제를 보장하지는 않는다. 동시성 문제를 완전히 해결해주지는 않음

- blocking io nonblocking io 에 대해 설명해주세요, system.out.println과 어떤 관계일까요?

blocking io : 입출력이 수행되는 동안 스레드는 대기상태에 있는다.  (System.out.println은 blocking io) <br>
non blockingn io : 입출력 작업을 수행하는 동안 호출자 스레드가 블록되지 않고 다른 작업을 수행하도록 한다.

- 스레드가 멈춰있으면 cpu는 어떻게 되나요? 스레드가 멈추면 Cpu는 다른 활성화된 스레드를 처리할 수 있습니다.
- cpu가 쉬는 것을 막으려면 어떻게 해야하나요? 멀티스레드를 활용해 병렬적으로 작업을 수행할 수 있도록 한다.
- 스레드를 늘리면 단점이 뭘까요? 스위칭 작업이 많이 일어나면 CPU 오버헤드가 발생한다. CPU코어가 정해져있는데 스레드가 많으면 자원을 가지기 위해 경쟁이 일어난다.
- 톰캣은 스레드를 어떻게 다루나요? 스레드 풀, 멀티 스레드, 요청-스레드 매핑 
- 객체의 불변성의 장점, 그리고 컬렉션에서는 불변성을 어떻게 다루는 지
- blocking nonblocking 차이 sync async와의 차이

## 혁준
- AutoCloseable, Closeable 차이점에 대해 설명하세요.
- static이 저장되는 위치는 어디인가요?
- Java 8이후로 Heap의 Permanent(PermGen) 영역이 Native Memory 영역의 Metaspace로 대체된 이유는?
- main 메서드가 static인 이유를 아시나요?
- 익명 클래스나 람다 표현식에서 외부 지역변수를 참조할 때, final 혹은 effective final이어야 하는 이유가 있나요?
- final은 완벽한 불변을 보장하나요?
- 그렇다면, 어떻게 불변성을 보장할까요?
- hashcode() 를 정의해야 한다면, 어떤 점을 염두에 두고 구현할 것 같으세요?
- equals() 를 재정의해야 할 때, 어떤 점을 염두에 두어야 하는지 설명해 주세요.
- Volatile에 대해 설명해주세요.
- 가시성이란 무엇인가요?
- Atomic에 대해 설명해주세요.
- String, StringBuffer, StringBuilder 차이점을 설명해주세요.
- `String a = ""`과 `String a = new String("")`의 차이점을 설명해주세요.

## 창현
- Checked Exception과 Unchecked Exception의 차이에 대해서 설명해주세요.
- static을 주로 언제 사용하시는지?
- static은 JVM 메모리의 어떤 영역에서 사용되는지?
- 병렬 처리는 항상 빠른가요? 병렬 처리에 영향을 미치는 요인을 말씀해주세요.
- 리플렉션을 사용해본 경험이 있으신지? 있으시면 설명해주시고, 없으시면 언제 사용할 것 같은지 얘기해주세요.
- Equals()와 Hashcode()에 대해서 설명해주세요.
- 동등성과 동일성에 대해서 설명해주세요.
- AtomicInteger가 무엇인지 설명해주세요. CAS는 무엇인가요?

## 범석
- static 키워드의 용도는 무엇인가요?
- final 키워드는 어떤 상황에 사용되며, 그 의미는 무엇인가?
- Checked Exception과 UnChecked Exception의 차이점에 대해서 설명해주세요
- Generic을 사용하는 이유는 무엇인가? 
- Stream API의 장점은 무엇인가? 
- 람다에 대해서 설명햊세요
- Java에서의 Collection은 무엇인가? 
- Thread safe 한 것은 어떤 의미를 하나요?
- equals(), hashcode의 정의와 주의점에 대해서 설명해주세요 
- Volatile 키워드는 무엇을 의미하나요? 
- String, StringBuffer, StringBuilder의 차이점에 대해서 설명해주세요 
- String 생성 시 literal 방식, 생성자 방식의 차이점에 대해서 설명해주세요
- [추가 질문]
  - 트랜잭션 체크 예외 언체크 예외 롤백 커밋의 전략이 정해주는 이유?
  - 병렬 스트림은 어떠한 방식으로 처리를 하게 되는지?
      - work stealing 알고리즘은 무엇인가
  - 람다에서 외부 참조 변수에 대해 effectively final 혹은 final 이어야 하는 이유는 무엇인지?
