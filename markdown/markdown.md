# :book: markdown 작성법

## 제목(heading)

제목은 문서의 구조와 관련이 있다.

'#'의 개수에 따라 제목의 중요도가 달라진다.

h1~h6까지 존재하며. #을 붙여서 표현 가능.

문서에 h1과 h3만 있다  => 문서를 잘못 작성한 것



## 목록(list)

### 순서있는 목록

문장 맨 처음에 1.하고 띄어쓰기 하면 작성시 자동으로 목록으로 바뀜

1. 수업을 한다
   1. 슬라이드 진행

1. 쉬는시간
2. 수업
3. 점심

### 순서없는 목록

문장 맨 처음에 -를 쓰고 띄어쓰기 하면 자동으로 바뀜

- git
  - ...
- CLI 명령어
  - 폴더
    - mkdir
    - rm -r
    - cd
  - 파일
    - touch
    - start
    - rm

- markdown 문법





## 본문 꾸미기(inline deco)

- 인용구(있어 보이는 말) --->    

- 나는 오늘 **github 특강**을 듣는다.

- git은 vcs이다.

- 인라인코드 :   `로 감싸기 
  - `폴더`를 `이동`할 때는 , `cd명령어`를 사용한다.

- **볼드** : **로 감싸기 or ctrl + B

- *기울이기*:  * or

## 코드블럭(code block)

backquote(backtic) 3개  + enter로 코드블럭 생성



```python
a = 1
b = 2
c = a + b
print(c)
```



 ## 표(table)

우클릭 + 삽입 (표)

​			or

pipe(|)로 열을 구분하고 Enter로 표 생성 ctrl +  Ennter로 행 추가



| 명령어  | 설명      | 사용 예시 |
| ------- | --------- | --------- |
| `mkdir` | 폴더 생성 | mkdir aaa |
| cd      | 폴더 이동 | cd. aaa   |
|         |           |           |



##  수식(Tex)

달러 2개로 블럭 생성. 내부작성법은 따로 학습


$$
\begin{align*}
y = y(x,t) &= A e^{i\theta} \\
&= A (\cos \theta + i \sin \theta) \\
&= A (\cos(kx - \omega t) + i \sin(kx - \omega t)) \\
&= A\cos(kx - \omega t) + i A\sin(kx - \omega t)  \\
&= A\cos \Big(\frac{2\pi}{\lambda}x - \frac{2\pi v}{\lambda} t \Big) + i A\sin \Big(\frac{2\pi}{\lambda}x - \frac{2\pi v}{\lambda} t \Big)  \\
&= A\cos \frac{2\pi}{\lambda} (x - v t) + i A\sin \frac{2\pi}{\lambda} (x - v t)
\end{align*}
$$


![image-20210705142114481](markdown.assets/image-20210705142114481.png)







