# Operator  
  
## ✅ Operator(연산자)란? 연산자는 데이터(변수, 상수 등)에 어떤 동작을 수행하는 기호  
  
일반 연산  
```
System.out.println(4 + 2); // 6
System.out.println(4 - 2); // 2
System.out.println(4 * 2); // 8
System.out.println(4 / 2); // 2
System.out.println(5 / 2); // 5를 2로 나눈 몫 = 2
System.out.println(2 / 4); // 0.5 -> 0
System.out.println(4 % 2); // 4를 2로 나눈 나머지 = 0
System.out.println(5 % 2); // 5를 2로 나눈 나머지 = 1
```
우선 순위 연산  
```
System.out.println(2 + 2 * 2); // 6
System.out.println((2 + 2) * 2); // 괄호 먼저 계산 = 8
```
변수를 사용한 증감연산  
```
int val;
val = 10;
System.out.println(val); // 10
System.out.println(++val); // 11
System.out.println(val); // 11

val = 10;
System.out.println(val); // 10
System.out.println(val++); // 10
System.out.println(val); // 11
```
++val 은 먼저 +1 계산 후 출력  
val++ 은 출력 후 +1 계산  


예제)  
은행 대기 번호 표  
```
int waiting = 0;
System.out.println("대기 인원 : " + waiting++); // 대기인원 : 0
System.out.println("대기 인원 : " + waiting++); // 대기인원 : 1
System.out.println("대기 인원 : " + waiting++); // 대기인원 : 2
System.out.println("총 대기 인원" + waiting); // 총 대기 인원 : 3
```

복합 대입 연산자  
```
num = 10;
num += 2;
System.out.println(num); // 12
```
num += 2 는 num = num + 2와 같다  

비교 연산자
```
System.out.println(5 > 3); // true
System.out.println(5 >= 3); // true
System.out.println(5 == 5); //true
System.out.println(5 != 5); //false
```
값이 참이면 true, 거짓으면 false가 나온다.  

논리 연산자  
And 연산  
```
System.out.println((5 > 3) && (3 > 1)); // 둘다 true 여야 true
System.out.println((5 > 3) && (3 < 1)); // 하나라도 false면 false
```
Or 연산  
```
 System.out.println((5 > 3) || (3 > 1)); // 하나라도 만족하면 true
System.out.println((5 > 3) || (3 < 1)); // 하나라도 true면 true
```
논리 부정연산자  
```
System.out.println(!true); // false
System.out.println(!false); // true
System.out.println(!(5 == 5)); // false
System.out.println(!(5 == 3)); // true
```
삼항 연산자  
```
int x = 5;
int y = 3;
int max = (x > y) ? x : y; // 참이면 x 거짓이면 y
System.out.println(max);
```
