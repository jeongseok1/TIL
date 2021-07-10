# 예외 처리

## 예외처리란?

예외 발생을 감지하고 복구하는 방법이다.

### 예외

s/w 로직에 의해 발생 --> 프로그램 종료
예외 처리를 하여 복구 가능

## 예외의 종류

- SyntaxError : 잘못된 문법
- NameError : 참조변수 없을 때
- ValueError : 참조 값이 없을 때
- IndexError : 인덱스 범위 벗어났을 때
- TypeError : 타입이 맞지 않을 때

## 예외처리 하기

### tyr except

#### try 

예외 발생 가능성이 있는 코드를 작성

#### except

예외가 발생할 경우 실행한다.  단, 예외 정보는 받지 못함

##### 어떤 예외가 발생할 지 예상 가능할 때 

except 뒤에 예외 정보를 입력한다.
ex) except ValueError   except IndexError

##### 어떤 예외가 발생할 지 모를 때

- **except:**
  - 모든 예외에 사용 가능하나 예외 정보를 받지 못한다. 
- **except Exception:**
  - except와 같은 의미로 모든 예외에 사용 가능하다.
  - 예외정보를 받을 수 있다.
  - 처음엔 이 형태로 운용하는 것 추천

- **except ~ as 변수명:**
  - 어떤 예외가 발생했는지 확인하고 싶은 경우 사용한다.
  - 예를 들어 `except Exception as e:` 라 쓰고 안에 `print(e)`를 출력하면 예외 내용을 확인할 수 있다.