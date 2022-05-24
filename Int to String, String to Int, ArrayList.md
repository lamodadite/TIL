### Int를 String으로 바꾸는 법

1. Integer.toString()

Integer 클래스의 toString() method를 사용한다.

```java
int a = 123;
String str = Integer.toString(a);
```

1. String.valueOf()

String 클래스의 valueOf() method를 사용한다.

```java
int a = 123;
String str = String.valueOf(a);
```

3) "" + n

java에서 문자열 오른쪽에 + operator를 붙이면(연산을 가하면) 새로운 문자열이 return 되는 속성을 이용한다

```java
int a = 123;
String string = "" + a;
```

### String을 Int로 바꾸는 법

1. Integer.parseInt()

Integer 클래스의 parseInt() method를 사용한다.

```java
String a = "123"
int intValue = Integer.parseInt(a);
```

1. Integer.valueOf()

Integer 클래스의 valueOf() method를 사용한다.

```java
String a = "123"
int intValue = Integer.valueOf(a).intValue();
```

뒤에 intValue() 메소드를 호출한 이유는

valueOf() 메소드가 primitive type으로 int를 반환하는것이 아니라, Integer Object를 리턴하기 때문이다. 

### String을 뒤집는법

StringBuffer로 바꾼 후에

reverse() 메소드를 이용한 후 다시 String으로 바꿔준다.

```java
String a = "123"
StringBuffer sb = new StringBuffer(a);
String reverse = sb.reverse().toString();
// 출력결과 = "321"
```

### ArrayList를 쓰는 이유 (동적 할당을 위해)

이거땜에 1분도 안걸릴 문제를 거의 1시간 동안 고민했다.

자바에서는 배열을 선언할때 배열의 크기를 꼭 선언해주어야 한다. 그리고 배열의 크기가 고정된다. 

하지만 원하는 결과의 배열의 크기를 아직 알 수 없다면? 매개변수에 따라 크기가 달라진다면?

이럴때 ArrayList를 써야한다. ArrayList는 객체가 추가되어 용량을 초과하면 자동으로 부족한 크기만큼 용량이 늘어난다. 

### 오늘 배운점

1. 자바는 정말..너무너무 strict하다..
2. 기본적인건 정확히 알고 있어야 빠르게 할 수 있다. int → string, 문자열 뒤집기, 이런 자료구조나 형변환은 꼭 숙지하고 익숙해지자. 
3. 코테를 볼 때 IDE를 못쓰게 할 수도 있다고 한다.. 절망적..
4. 내일은 기초수학 꼭 끝내자.
