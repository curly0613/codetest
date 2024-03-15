# codetest
## 코드테스트에서 유용한 python 내장 함수들

1. upper() : 문자열 알파벳 대문자로
   ```
   'abc'.upper()
   'ABC'
   ```
2. lower() : 문자열 알파벳 소문자로
3. swapcase() : 대소문자 변경
4. zip() : for문 시 여러 리스트의 원소를 각 하나씩 loop
5. join() : list를 문자열로 출력
   ```
   ''.join(list)
   ```
6. 비교 연산자 차이 
  - is 와 == : is는 주소비교, =는 값 비교
  - and 와 & : and는 논리연산자, &는 bitwise 비교
  - or 와 | : or는 논리연산자, |는 bitwise 비교
7. 수치적 표현
  - 제곱 : a ** 2, a ** 3
  - 절대값 : abs()
8. lambda
  - 함수 대용, 간단한 함수 정의
  - example
    ```
    lambda x,y:x+y
    (lambda x,y:x+y)(1,2)
    3
    map(lambda x:x*2, range(5))
    [0, 2, 4, 6, 8]
    ```
