# python 정리

## lambda 함수

### 정의

```
def 함수명(  ):
    
    문장
```
을 다르게 표현하는 표현식

### 주의

단일 문장만 람다 표현식으로 변환 가능하다.

## 일급객체(first-class)

### 개념

기능 담당하는 함수를 정수 및 문자열과 같은 데이터로 처리한다.

### 특징

- **함수는 Data가 맞다.**

---

- 함수는 변수에 저장 가능하다. 
  ```
  def fun():
    print("fun")

  print(fun)
  n=fun
  n()
  ```
  변수 n에 함수로 정의된 fun 저장      

- 함수를 함수 호출시 인자값으로 사용이 가능하다.
  ```
  def x():
    print("x")

  def y(n):
    n()

  y(x)
  ```
  함수 x를 함수 y 호출 시 인자값으로 이용

- 함수를 함수 리턴값으로 사용 가능하다.
    ```
    def k():
        print("k")

    def k2():
        return k

    result = k2()
    result()
    ```
