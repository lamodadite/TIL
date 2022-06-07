## IntStream

`IntStream.*of*(arr).forEach(x -> deque.addLast(x));`

- int[] arr 배열을 스트림 형태로 만들고
- forEach로 원소를 순서대로 요리 가능

### Stream

`result.stream().mapToInt(x -> (int)x).toArray()`

- result라는 ArrayList를 스트림으로 바꾼다
- 각 원소들을 모두 int로 바꿔서
- toArray로 배열로 만들어서 출력

> 스트림은 데이터 소스로 부터 데이터를 읽기만 할 뿐, 변경하지 않는다.
> 

> 스트림은 한 번 사용하면 닫혀서 다시 사용할 수 없다.
> 

> 스트림은 작업을 내부 반복으로 처리한다.
>
