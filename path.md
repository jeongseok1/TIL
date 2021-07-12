# path(경로)

파일(폴더)의 위치를 나타내는 문자열
트리 구조를 따르며 최상위 폴더는 root 폴더(디렉토리)이다.

```
tree 구조 == 계층 구조
    상위 == 부모
    하위 == 자식
```

current working directory(cwd) : 현재 워킹 디렉토리

home directory : 로그인 했을 때 가지는 디폴트 워킹 디렉토리

## 절대경로(absolute path)

root에서 시작되는 경로

## 상대경로(relative path)

cwd에서 시작되는 경로



> cwd --> c:\temp\ttt 가정하면

>  test_a  ---> 상대경로

>  c:\temp\ttt\test_a



최상위폴더(\, 루트 디렉토리)부터 시작하면 절대경로

\temp\test_a  --> 절대 경로



## windows 경로

​	드라이브:최상위폴더

​	c:\temp\a.txt

​	c:\temp\test_a

​	c:\temp\test_a\c.txt



## 기타

.   : 자기 자신
..  : 상위 폴더/부모 폴더