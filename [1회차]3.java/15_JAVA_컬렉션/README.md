 - JAVA 컬렉션
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

## 질문

### 재현
- 왜 우리는 arrayList를 사용하면서도 타입은 list로 사용할까요?
- concurrentHashMap이 왜 hashTable에 대해서 더 빠를까?
- treeMap의 특징을 설명해줄 수 있을까요 => 레드블랙 트리에 대해서 설명해줄 수 있을까요?
- Arrays.sort(), Collections.sort() 의 정렬 알고리즘에 대해 알고 있다면 설명 부탁드립니다.(퀵정렬)
- hashTable보다 conCurrentHashMap이 더 빠른 이유
- hashtable, hashmap, likedHashMap, treeMap의 특징을 종류별로 설명해주세요
- linkedList, arrayList를 비교해서 설명해주세요
- stringBuffer,StringBuilder를 비교해서 섦여해주세요
- string이 불변인 이유에 대해 설명해주세요
- 스레드의 안정성을 고려할 수 있는 방법에 대해 설명해주세요
- 불변성을 보장하는 방법에 대해 일반 객체, array, list의 경우에 대해서 설명해주세요
- 해시 충돌에 대해서 설명해주세요

### 창현
- ThreadSafe이 무엇을 말하는지 설명해주세요.
- Syncronized를 사용하기 위한 방법 2가지에 대해서 설명해주세요.
- Syncronized의 단점과 이를 극복하기 위한 방법에 대해서 알려주세요.
- String은 StringBuffer/StringBuilder와 무슨 차이가 있을까요?
- StringBuffer와 StringBuilder는 무슨 차이가 있을까요?
- 불변 객체의 장점에 대해서 설명해주세요
- ArrayList와 LinkedList의 차이점에 대해서 설명해주세요.
- HashTable과 HashMap, LinkedHashMap, TreeMap에 대해서 간단하게 설명해주세요.
- HashMap과 ConcurrentHashMap의 차이에 대해서 알려주세요.

### 범석
- thread - safe은 무엇인가요? 
- synchronized 키워드가 붙었을 때 어떻게 동작하는지, 어떻게 사용할 수 있는지 설명해주세요. 
- String, StringBuilder, StringBuffer에 대해서 설명해주세요 
- 불변 객체는 무엇인가요? 
- 알고 있는 불변 객체에 대해서 설명해주세요 
- 일반 클래스를 불변객체로 만들기 위해서는 어떻게 해야할 까요? 
- ArrayList LinkedList는 각각 내부적으로 무엇을 통해 구현이되어있는지 설명 부탁드립니다. 
- ArrayList LinkedList 중간에 원소를 삽입 / 삭제할 경우 시간 복잡도는 어떻게 되나요? 
- HashTable vs HashMap vs LinkedHashMap vs TreeMap 에 대해서 간단한 특징 소개 부탁드립니다. 
- HashMap과 ConcurrentHashMap의 차이에 대해서 설명 부탁드립니다.

### 현호
- ArrayList와 LinkedList의 차이점은 무엇이며, 어떤 상황에서 어떤 자료구조를 선택해야 할까요?
- 여러 문자열을 합쳐서 하나의 문자열로 만들 때 String을 쓰는 경우와 StringBuilder를 쓰는 경우의 동작방식이 어떻게 다른지 설명해주세요.
- String a = ""와 String a = new String("")의 차이는 무엇이며, 어떤 상황에서 어떤 방법을 사용해야 할까요?
- ArrayList와 LinkedList의 시간 복잡도에 대해 설명하고, 이에 기반하여 어떤 상황에서 어떤 자료구조를 사용해야 할까요?
- HashMap, ConcurrentHashMap, LinkedHashMap, TreeMap의 차이점과 각각의 특징을 설명해주세요.
- HashMap이 키와 값으로 이루어진 하나의 Entry를 저장하는 과정을 최대한 자세히 설명해주세요.
- ConcurrentHashMap이 내부적으로 어떻게 동기화 처리를 하였는지 말씀해주세요.