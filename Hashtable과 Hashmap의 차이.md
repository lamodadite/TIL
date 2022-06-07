### Hashtable과 HashMap의 차이

- 공통점
    - 둘 다 Map 인터페이스를 구현한 것임
- 차이점
    - Key에 Null값 사용 가능 여부
        - hashtable 은 불가능, hashmap은 가능
    - Thread-safe 여부
        - hashtable은 멀티 스레드 환경에서 우수
        - hashmap은 싱글 스레드 환경에서 우수
            - synchronizedMap, ConcurrentHashMap을 쓰면 hashmap도 thread-safe하게 사용 가능하다
