# class

## class란

관련 정보(변수)와 정보의 조작 함수(메서드)를 묶어서 관리하는 것

여러 데이터를 관리할 때  함수만 쓰는것 보다 편리하다.

## class 정의

`class 키워드` 로 정의하고 이때 클래스 이름(키워드)은 파스칼표기법(단어의 앞글자가 대문자로 시작)으로 작성한다.

사용하기 위해서는 인스턴스를 생성한 후 사용해야 한다.

```python
# ex)
class NameCard:
    def __init__(self):	# 생성자 함수
        pass
name = NameCard()	# NameCard의 인스턴스 생성
```

