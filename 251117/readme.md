# 📘 IoT Python Programming – Chapter 1 Summary  
*Based on Lecture PDF: "제1장 파이썬 소개"*  
<학습 요약 저장용 README>

---

## 📙 1. 컴퓨터와 프로그램

- 컴퓨터는 유연한 기계이며, 다양한 작업을 처리할 수 있음
- 컴퓨터에게 일을 시키려면 **명령어의 집합(Program)** 이 필요함
- 프로그램은 인간이 작성 ➜ 컴퓨터가 수행

---

## 🧠 2. 프로그래밍을 배워야 하는 이유

- 모든 산업 분야에서 필수 기술이 되고 있음
- AI 로봇, 자동 주식 매매, RPA 등 자동화 시대 핵심 역량
- 컴퓨터는 인간이 귀찮아하는 반복 업무에 매우 강함

---

## 💬 3. 프로그래밍 언어 & 실행 방식

### ● 프로그래밍 언어
- 컴퓨터가 이해하는 언어
- 대표적 언어: **Python, Java, C, BASIC …**
- 프로그램을 작성하는 사람 → “프로그래머”

### ● 컴파일러 / 인터프리터
- 인간이 작성한 코드를 기계어로 번역하는 소프트웨어
- 파이썬은 인터프리터 방식 → 즉시 실행 결과 확인 가능

---

## 🐍 4. 파이썬(Python) 소개

- 1991년 귀도 반 로섬이 개발
- **간결 + 생산성 + 풍부한 라이브러리**
- 초보자에게 매우 적합한 언어

---

## 🛠 5. 개발 환경 – Anaconda & Spyder

- 아나콘다: 주요 라이브러리가 포함된 파이썬 배포판
- Spyder: 파이썬 기반 IDE (코드 편집 + 실행 + 디버그)
- 실행 모드
  - **대화형 모드**: 한 줄씩 실행
  - **스크립트 모드**: .py 파일 저장 후 한 번에 실행

---

## 🖥 6. 기본 문법 예시

```python
print("Hello Python")
print("2+3=", 2+3)
print("Hello" * 10)   # 문자열 반복
```

## 🐢 7. 터틀 그래픽(Turtle)
import turtle
t = turtle.Turtle()
t.shape("turtle")
t.forward(100)
t.left(90)
turtle.mainloop()


파이썬 내장 그래픽 기능

교육용 시각 실습에 적합

## 🧪 8. 실습 예제 리스트

print() 함수로 문장 출력하기

간단한 사칙연산 출력

문자열 반복 출력

오류 고쳐보기 실습

터틀 그래픽으로 삼각형 그리기

📌 핵심 정리
개념	내용
프로그램	컴퓨터가 수행할 명령어 집합
프로그래밍 언어	컴퓨터가 이해하는 언어
파이썬 특징	간결, 대화형, 라이브러리 多
인터프리터	즉시 실행 방식
print()	출력 함수
스크립트 모드	파일(.py) 실행 방식


# 📘 IoT Python Programming – Chapter 2 Summary  
**주제: 변수와 수식 기본 개념 정리**

> 본 문서는 수업 교재 **「제2장 변수와 수식(강의).pdf」** 내용을 요약한 학습 정리 자료입니다.  
> :contentReference[oaicite:0]{index=0}

---

## 🎯 학습 목표

- 변수와 상수 정의 및 사용
- 주석(comment) 개념 이해
- 산술·할당 연산자, 연산자 우선순위
- `input()` / `print()` 사용법
- 문자열 기본 연산
- 사용자 입력 기반 간단한 프로그램 작성

---

## 🧩 1. 변수 (Variable)

- 변수 = **값을 저장하는 이름 있는 메모리 공간**
- 파이썬은 **변수 선언 없이 대입하면 자동 생성**

```python
x = 100
y = 200
sum = x + y
```

✔ 변수 이름 규칙

영문자, 숫자, 밑줄(_) 가능

숫자로 시작 ❌

대문자/소문자 구별

의미 있는 이름 권장

myVariable ← 카멜 표기법

🧮 2. 자료형(Data Types)
타입	예시	특징
int	10	정수
float	3.14	실수
str	"Hello"	문자열
bool	True/False	논리형

확인 방법:
```python
type(3.14)   # <class 'float'>
```

🔁 3. 산술 연산자
연산	의미
+	덧셈
-	뺄셈
*	곱셈
/	실수 나눗셈
//	정수 몫
%	나머지
**	지수

예시:
```python
7 // 4   # 1
7 % 4    # 3
2 ** 7   # 128
```

🏷 4. 할당 & 복합 대입 연산
```python
x = 10
x += 5   # 15
x *= 2   # 30
x, y = 10, 20  # 동시 할당
x, y = y, x    # 변수 교환
```

⚖ 5. 연산자 우선순위

📌 곱셈/나눗셈 > 덧셈/뺄셈
```python
10 + 20 / 2  # 20.0
(10 + 20) / 2 # 15.0
```

📝 6. 주석(Comment)
```python
# 한 줄 주석
"""
여러 줄 주석 (문자열 활용)
"""
```

🔤 7. 문자열(String)
기능	예시
결합	"Hi" + "Python"
반복	"=" * 30
인덱싱	"Hello"[0] → 'H'
치환	"Hi".replace("H","Y")

문자열 <-> 숫자 변환:
```python
int("100")   # 100
str(100)     # "100"
float("3.14")  # 3.14
```

⌨ 8. 사용자 입력 input()
```python
name = input("이름: ")
x = int(input("정수 입력: "))
y = float(input("실수 입력: "))
```

💡 대표 실습 예시
✔ BMI 계산
```python
weight = float(input("몸무게(kg): "))
height = float(input("키(m): "))
bmi = weight / (height ** 2)
print("BMI=", bmi)
```

✔ 자동판매기 거스름돈 계산
```python
item = int(input("물건값: "))
money = int(input("지불금액: "))
change = money - item
print("500원:", change//500)
```

🧪 Lab 목록 요약
실습	내용
원 면적 계산	radius → area
별까지 거리	빛의 속도 기반 연산
삼각형/정사각형 그리기	turtle 사용
문자열 기사 생성	input + 출력
BMI 계산	실수 입력 & 연산
자판기 거스름돈	//, % 활용


# 📘 IoT Python Programming – Chapter 3 Summary  
**주제: 조건문 (if, elif, else)**  
**출처:** 제3장 조건문(강의).pdf  
:contentReference[oaicite:0]{index=0}

---

## 🎯 학습 목표

- 제어문의 개념 이해
- `if`, `elif`, `else` 구조 사용
- 관계·논리 연산자 활용
- 블록(들여쓰기) 개념 이해
- 중첩 조건문 & 연속 조건문 작성

---

## 🧭 1. 제어문(Control Structure)

### ✔ 프로그램 실행 흐름을 바꾸는 구조

| 종류 | 설명 |
|------|------|
| 순차 구조 | 위 → 아래로 실행 |
| **조건문** | 조건에 따라 실행 경로 변화 |
| 반복문 | 특정 문장을 반복 실행 |

조건문이 없다면 프로그램은 항상 동일한 결과만 수행하게 됨

---

## 🧩 2. if-else 기본 구조

```python
if 조건식:
    실행문1
else:
    실행문2

🔎 3. 관계 연산자
연산자	의미
==	같다
!=	같지 않다
>, <	비교
>=, <=	이상 / 이하

✔ 결과는 항상 True / False (부울값)

🧠 논리 연산자
연산자	의미
and	모두 참
or	하나만 참
not	반대로

📌 not (A and B) 🔁 (not A) or (not B)
→ 드모르간 법칙

🔀 4. 조건 연산자 (삼항 연산자)
result = (값1 if 조건 else 값2)


예시:

shipping_cost = (0 if price > 20000 else 3000)

🏷 5. 문자열 / 실수 비교

✔ 문자열은 사전 순 비교 가능
✔ 실수 비교 시 == 직접 비교 ❌
➡ abs(a-b) < 작은값 형태 권장

🧱 6. 중첩 if 문
if country == "korea":
    if price >= 20000:
        cost = 0
    else:
        cost = 3000
else:
    if price >= 100000:
        cost = 0
    else:
        cost = 8000

🔁 7. 연속 if-elif-else
if score >= 90:
    print("A")
elif score >= 80:
    print("B")
elif score >= 70:
    print("C")
else:
    print("F")

🧪 대표 Lab 실습 목록
Lab	개념 활용
산술 퀴즈	==, 랜덤
짝수/홀수	%
세일 가격 계산	조건 연산자
물의 상태 출력	elif
동전던지기	랜덤 + if
리히터 규모 판별	연속 if
메뉴 선택 검증	논리 연산
축구 게임	사용자 입력 + 랜덤
8 매직볼	난수 + 조건문
올바른 삼각형	세 조건 AND
터틀 도형 그리기	조건문 + 그래픽
🧩 예제 코드 모음
✔ 짝수 / 홀수 판별
n = int(input("정수를 입력하시오: "))
print("짝수" if n % 2 == 0 else "홀수")

✔ 리히터 규모 예제
scale = float(input("리히터 규모: "))
if scale >= 8: print("대부분의 구조물 파괴")
elif scale >= 7: print("지표면 균열")
elif scale >= 4: print("빈약한 건물 피해")
elif scale >= 2: print("물건 흔들림")
else: print("기계만 탐지 가능")

📌 핵심 정리

제어문 = 조건문 + 반복문

if-elif-else 구조를 들여쓰기로 표현

조건문 내부에서 변수·수식·부울 변수 사용 가능

논리 연산으로 복합 조건 설정 (and,or)

실수 비교는 abs 사용

조건문은 중첩 가능하며 구조화가 매우 중요함

