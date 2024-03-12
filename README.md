# Python

## Python Syntax
##### 공백 없으면 오류 발생 
##### 일반적으로 4개 공백 사용됨 
##### 적어도 하나 필수
```
if 5 > 2:
  print("Five is greater than two!")
```
##### 변수에 값 할당 -> 변수 생성
```
x = 5
y = "Hello, World!"
```
##### #은 주석
```
#This is a comment.
```
---
## Python Comments
##### Python은 주석 뒤 무시
```
#This is a comment
print("Hello, World!")
```
---
## Python Variables
##### 다른 유형으로 변수 설정 가능
```
x = 5
y = "John"
print(x)
print(y)
```
##### 변수는 보다 길게 설정 가능 (다음처럼 설정 가능)
```
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
```
##### 또한 여러 값으로 설정 가능
```
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```
##### 여러 변수는 쉼표로 구분하거나 연산 가능 (수와 문자는 연산 불가)
```
x = "Python"
y = "is"
z = "awesome"
print(x, y, z)
```
```
x = "Python "
y = "is "
z = "awesome"
print(x + y + z)
```
---
## Python Data Types
```
문자열 유형: str
숫자(정수,실수) 유형: int, float, complex
시퀀스 유형: list, tuple, range
매핑 유형: dict
세트 유형: set,frozenset
부울 유형: bool
바이너리 유형: bytes, bytearray, memoryview
없음 유형: NoneType
```
##### type() -> 데이터 유형 추출
```
x = 5
print(type(x))
```
---
## Python Numbers
##### Python의 세가지 숫자 유형
```
int 정수
float 실수
complex 복소수

x = 1    # int
y = 2.8  # float
z = 1j   # complex
```
---
## Python Casting
##### 변수 유형 지정
```
정수
x = int(1)   # x will be 1
y = int(2.8) # y will be 2
z = int("3") # z will be 3

실수
x = float(1)     # x will be 1.0
y = float(2.8)   # y will be 2.8
z = float("3")   # z will be 3.0
w = float("4.2") # w will be 4.2

문자열
x = str("s1") # x will be 's1'
y = str(2)    # y will be '2'
z = str(3.0)  # z will be '3.0'
```
---
## Python Strings
##### '나 "로 표현
```
print("Hello")
print('Hello')
```
##### 슬라이스 구문 사용 -> 문자 반환
```
b = "Hello, World!"
print(b[2:5])

b = "Hello, World!" #처음부터
print(b[:5])
```
##### 변환
```
a = "Hello, World!" #소문자로
print(a.lower())

a = " Hello, World! " #공백 제거
print(a.strip()) # returns "Hello, World!"

a = "Hello, World!" #문자열 바꾸기
print(a.replace("H", "J"))

a = "Hello, World!" #문자열 분할
print(a.split(",")) # returns ['Hello', ' World!']
```
##### 연결
```
a = "Hello"
b = "World"
c = a + b
print(c)

a = "Hello" #공백 추가
b = "World"
c = a + " " + b
print(c)
```
##### 형식 지정
```
age = 36
txt = "My name is John, and I am {}"
print(txt.format(age))

quantity = 3
itemno = 567
price = 49.95
myorder = "I want {} pieces of item {} for {} dollars."
print(myorder.format(quantity, itemno, price))

quantity = 3
itemno = 567
price = 49.95
myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
print(myorder.format(quantity, itemno, price))
```
##### 이스케이프 문자
```
txt = "We are the so-called \"Vikings\" from the north."
```
---
## Python Booleans
##### True 또는 False 출력
```
print(10 > 9)
print(10 == 9)
print(10 < 9)

a = 200
b = 33
if b > a:
  print("b is greater than a")
else:
  print("b is not greater than a")

print(bool("Hello"))
print(bool(15))

x = "Hello"
y = 15
print(bool(x))
print(bool(y)
```
---
## Python Operators
##### 연산에는 + 사용
```
print(10 + 5)
```
---
## Python Lists
##### 목록은 단일 변수에 여러 항목 저장
##### 변경 가능
##### 중복 허용
##### 목록 길이 -> len()
##### 목록 항목은 모든 데이터 유형 가능
##### type()
##### list()
```
thislist = ["apple", "banana", "cherry"]
print(thislist)

thislist = ["apple", "banana", "cherry", "apple", "cherry"]
print(thislist)

thislist = ["apple", "banana", "cherry"]
print(len(thislist))

list1 = ["apple", "banana", "cherry"]
list2 = [1, 5, 7, 9, 3]
list3 = [True, False, False]

list1 = ["abc", 34, True, 40, "male"]

mylist = ["apple", "banana", "cherry"]
print(type(mylist))

thislist = list(("apple", "banana", "cherry")) # note the double round-brackets
print(thislist)
```
---
## Python If ... Else
##### if문 종류
```
Equals: a == b
Not Equals: a != b
Less than: a < b
Less than or equal to: a <= b
Greater than: a > b
Greater than or equal to: a >= b
```
---
## Python While Loops
##### 두 가지 기본 루프 명령
```
while 루프
for 루프
```
##### while 루프
##### break 문
##### 계속 진술
##### else 문
```
i = 1
while i < 6:
  print(i)
  i += 1

i = 1
while i < 6:
  print(i)
  if i == 3:
    break
  i += 1

i = 0
while i < 6:
  i += 1
  if i == 3:
    continue
  print(i)

i = 1
while i < 6:
  print(i)
  i += 1
else:
  print("i is no longer less than 6")
```
---
## Python For Loops
##### for 루프 -> 시퀀스(목록, 튜플, 사전, 집합 또는 문자열) 반복
```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
```
##### 문자열을 통한 반복
```
for x in "banana":
  print(x)
```
##### break 문
```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break

fruits = ["apple", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    break
  print(x)
```
##### 계속 진술
```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    continue
  print(x)
```
##### range() 함수
```
for x in range(6):
  print(x)

for x in range(2, 6):
  print(x)

for x in range(2, 30, 3):
  print(x)
```
##### For 루프의 Else
```
for x in range(6):
  print(x)
else:
  print("Finally finished!")

for x in range(6):
  if x == 3: break
  print(x)
else:
  print("Finally finished!")
```
##### 중첩 루프
```
adj = ["red", "big", "tasty"]
fruits = ["apple", "banana", "cherry"]

for x in adj:
  for y in fruits:
    print(x, y)
```
##### 패스 설명
```
for x in [0, 1, 2]:
  pass
```












