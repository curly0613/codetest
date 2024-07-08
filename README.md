# codetest
## 코드테스트에서 유용한 python 내장 함수들

1. upper() : 문자열 알파벳 대문자로
   ```
   > 'abc'.upper()
   > 'ABC'
   ```
2. lower() : 문자열 알파벳 소문자로
3. swapcase() : 대소문자 변경
4. zip() : for문 시 여러 리스트의 원소를 각 하나씩 loop
5. join() : list를 문자열로 출력
   ```
   > list = [a, b, c, d, e, f, g]
   > ''.join(list)
   > 'abcdefg'
   ```
6. 비교 연산자 차이
   - is 와 == : is는 주소비교, =는 값 비교
   - and 와 & : and는 논리연산자, &는 bitwise 비교
   - or 와 | : or는 논리연산자, |는 bitwise 비교
8. 수치적 표현
   - 제곱 : a ** 2, a ** 3
   - 절대값 : abs()
10. lambda
    - 함수 대용, 간단한 함수 정의
    - example
      ```
      > lambda x,y:x+y
      > (lambda x,y:x+y)(1,2)
      > 3
      > map(lambda x:x*2, range(5))
      > [0, 2, 4, 6, 8]
      ```
11. double colon
    - step을 의미
      ```
      > A = [1, 2, 3, 4, 5]
      > A[::2]
      > [1, 3, 5]
      > A[::-1]
      > [5, 4, 3, 2, 1] 
      ```
12. startswith, endswith
    - 접두사, 접미사 확인
    - rfind, rindex : 문자열에서 마지막으로 나타나는 특정 문자 또는 문자열의 index
13. count
    - 문자열의 문자 개수 반환
      ```
      > 'abcda'.count('a')
      > 2
      ```
14. strip, lstrip, rstrip
    - 인자로 받은 문자열을 제거(strip: 양쪽, lstrip: 왼쪽, rstrip: 오른쪽)
15. bin
    - 10진수를 2진수로 변형 (문자열, 앞에 0b가 붙음)
      ```
      > bin(10)
      > '0b1010'
      ```
16. *arr
    - 배열을 풀어서 나열 (zip과 함께 사용하면 열 기준 배열 생성 가능)
      ```
      > *[a, b, c]
      > a b c
      >
      > list(zip(*[[1,1],[2,2]]))
      > [(1,2),(1,2)]
      ```
17. heapq
    - heap queue 구현
    - heappush, heappop
18. itertools
    - 순열, 조합 구현
    - permutations, combinations
19. dictinary의 value 최대값
    - 최대 value를 갖는 key : max(dict, key=dict.get)
    - 하나 이상의 key를 출력할 때 : [key for key in dict if dict[key] == max(dict.values())]
