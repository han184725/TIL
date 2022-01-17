# Python basic

- 컴퓨터 프로그래밍 언어 -> 컴퓨터에게 명령하기 위한 약속
  - 선언적 지식: 사실에 대한 내용
  - 명령적 지식: how-to
- expressive language
- 크로스 플랫폼 언어
- 인터프리터 언어
- 객체 지향 프로그래밍
- 기본 인터프리터: IDLE(Integrated development and Learing environment)
- IDE: 통합 개발 환경
- 변수: 객체를 참조하기 위해 사용되는 이름
  - type(): 변수에 할당된 값의 타입
  - id(): 변수에 할당된 객체의 고유한 값(메모리주소)
  - 숫자+숫자, 문자+문자 가능
  - 같은 값 동시 할당 가능 `x=y=2`
  - 다른 값 동시 할당 가능`x,y=1,2`
  - 식별자: 이름(알파벳, 언더스코어, 숫자), 첫 글자에 숫자X, 대소문자 구별, 내장함수나 모듈 이름 X
  - input()
- 자료형
  - NoneType: 값이 없음
  - Boolean: True/False(비어있는 것 포함)->`bool()`
  - Int: 모든 정수, 매우 큰 수를 나타낼 때 오버플로우X(0b:2진수, 0o:8진수, 0x:10진수)
  - float: 실수 -> Floating point rounding error: 부동소수점에서 실수 연산 과정에서 발생 가능 ->`abs(a-b)<=1e-10`
  - String: Immutable, Iterable, Escape sequence(\n:엔터, \t:탭), String Interpolation(%-formatting, `str.format()`, f-strings)
- 컨테이너: 서로 다른 자료형을 저장 가능(List(가변),turple)
  - 순서 중요(순서=정렬)
  - 리스트: array(대괄호)
    - `len()`: 리스트 길이
  - 튜플: 소괄호, 불변, (())/`tuple()`->접근: `my_tuple[i]`
    - 파이썬 내부에서 활용

- 레인지( range): 숫자의 시퀀스
- 패킹, 언패킹
- 셋(Set): 해시 가능한 객체만, 삽입 변경 삭제 가능(가변), 집합과 동일, 중복없이 순서가 없는 자료구조 -> 리스트 내에서 고유한 개수: `len(set(list))`(->set사용시 순서 사라짐)
- 딕셔너리(dictionary): 키-값 쌍으로 이뤄진 객체 참조
  - key: 해시가능한 불변 자료형만 가능
  - {}, `dict()`로 생성, key를 통해 value 접근
- 형 변환(Typecasting): 데이터 형태 변환 가능
  - 암시적 형 변환(Implicit): 의도X, 내부적
  - 명시적 형 변환(explicit): 사용자 의도적
- 연산자(Operator)
  - //: 몫, %: 나머지
  - and연산에서 첫번째 값이 False인 경우 무조건 False(첫번째 값 반환)
  - or 연산에서 첫번째 값이 True인 경우 무조건 True(첫번째 값 반환)
  - in/not in
  - 시퀀스형 연산자: +, *
  - 슬라이싱: s[::], s[::-1]

***

string: 문자열의 나열

set:중복 없음

tuple:변경 불가한 요소들의 시퀀스

list: 요소들의 시퀀스

{k,v}:key value

숫자: boolean, none

패키지->라이브러리



***

c\users\name : 홈 경로, ~

언패킹: 튜플 형태(불변)

패킹: 리스트

***

`for char in chars`

`	print(char)`  (순회)

`for idx in range(len(chars))`

`	print(idx)` (인덱스(iterable))



딕셔너리 순회: key를 순회, key를 통해 값을 활용

`print(grades.keys())`: 

`print(grades.values())`

`print(grades.items())` : (key,value)의 튜플로 구성된 결과

`enumerate()` : 인덱스와 객체를 쌍으로 담은 열거형 객체 반환, (index, value) 형태 튜플로 구성된 열거 객체 반환

-> `list(enumerate())` 

x=[]

x.append(i)

x=[i for ~ if ]

print(x)



***

반복문 제어: brak, continue, pass

for: 반복 가능한 애들을 꺼내준다

while: 조건이 참일 때 실행





