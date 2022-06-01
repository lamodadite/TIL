### String에서 equals와 ==의 차이점

- equals 메소드는 비교하고자 하는 대상의 내용 자체를 비교
- == 연산자는 대상의 주소값을 비교

때문에 

`String a = “aaa”`

`String b = a`

`String c = “aaa”`

일때

a == b 는 true 지만

a == c 는 false이다. (주소값을 비교하기 때문에)

a.equals(c)는 true이다. (대상을 비교하기 때문에)
