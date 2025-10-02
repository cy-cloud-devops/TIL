# 🐍 파이썬 조건문 시리즈 (1~3탄)

---

## 🔹 1탄: If / Else 기본

### 🧩 예제 1: 양수/음수 판별
```python
num = int(input("숫자 입력: "))

if num > 0:
    print("양수입니다.")
else:
    print("음수 또는 0입니다.")
```

![양수/음수 판별 캡처](.assets/python/ifelse1.png)

**실행결과:**
```
숫자 입력: -3
음수 또는 0입니다.
```

---

### 🧩 예제 2: 합격/불합격 판별
```python
score = int(input("점수 입력: "))

if score >= 60:
    print("합격입니다!")
else:
    print("불합격입니다.")
```

![합격/불합격 캡처](.assets/python/ifelse2.png)

**실행결과:**
```
점수 입력: 58
불합격입니다.
```

✅ 포인트 정리  
- `if` 조건이 True면 실행, 아니면 `else` 실행  
- 가장 기본 구조  

---

## 🔹 2탄: If / Elif / Else 확장

### 🧩 학점 판별
```python
score = int(input("점수 입력: "))

if score >= 90:
    print("A 학점")
elif score >= 80:
    print("B 학점")
elif score >= 70:
    print("C 학점")
elif score >= 60:
    print("D 학점")
else:
    print("F 학점")
```

![학점 판별 캡처](.assets/python/ifelse3.png)

**실행결과:**
```
점수 입력: 83
B 학점
```

✅ 포인트 정리  
- 조건이 여러 개일 때 `elif` 사용  
- 위에서부터 차례대로 검사 → True 걸리면 뒤 조건은 검사 안 함  

---

## 🔹 3탄: 조건문 응용

### 🧩 세 수 중 가장 큰 수 찾기
```python
a = int(input("첫 번째 숫자: "))
b = int(input("두 번째 숫자: "))
c = int(input("세 번째 숫자: "))

if a >= b and a >= c:
    print("가장 큰 수:", a)
elif b >= a and b >= c:
    print("가장 큰 수:", b)
else:
    print("가장 큰 수:", c)
```

![세 수 중 최댓값 캡처](.assets/python/ifelse4.png)

**실행결과:**
```
첫 번째 숫자: 12
두 번째 숫자: 7
세 번째 숫자: 12
가장 큰 수: 12
```

✅ 포인트 정리  
- `and`, `or` 같은 논리 연산자 등장  
- 복합 조건 다룰 줄 알아야 실무에서 쓰임  

---

## ✨ 오늘의 회고
- `if / else`는 가장 기본이지만, 작은 조건 하나로도 프로그램 흐름이 확 달라지는 걸 직접 확인했다.  
- `elif`를 배우면서 “조건을 순서대로 평가한다”는 걸 이해했고, 실수로 범위를 잘못 잡으면 원하는 결과가 안 나온다는 점을 깨달았다.  
- `and`, `or` 응용까지 해보니 조건이 많아질수록 코드 구조를 잘 설계하는 게 중요하다는 걸 느꼈다.  
- 단순히 코드만 따라치는 게 아니라 **“왜 이렇게 동작하는지”**를 계속 떠올리면서 연습하는 게 핵심! 🚀 
