# MQTT

image/video/audio 등은 부적합 작은 파일정도는 가능

주로 센서 데이터등 전송

## 와일드카드문자

+, #

`+`  : 1레벨 모두
"센서/hong/+/temp"

`#`
"센서/hong/#"

## QoS(Quality of Service)

3단계 제공

0 : 전달여부를 확인하지 않는다. / ip프로토콜과 비슷/ 속도 높음 신뢰도 낮음

1 : 전송 후 메시지 받음 /중복전송될수있음 

2: 한 번만 전달 / 속도 낮음 신뢰도 높음

아두이노 : 0,1 가능

pc : 전부 다 가능



**m**os**q**ui**tt**o : 모기  mqtt가 들어있는 단어





## NodeMcu MQTT



### PubSubClient

라이브러리 설치

- Qos 0,1만 지원
- 1개의 topic만 subscribe 
  -  `#`,`+`지원안됨

#### void callback()

payload = 값, length = payload의 길이



memcpy

memcpy(dest,src,length)

dest에 src를 length만큼 복사



#### reconnect()

mqtt브로커에 연결

while(!client.connected())  

- 연결여부 
  - T : 연결 
  - F : 비연결

! 있으므로 비연결일때 실행







## mqtt_python

파이썬으로 mqtt

### paho모듈

#### 순서

1. 클라이언트 클래스 인스턴스화 하기
2. 핸들러 등록
3. 브로커 연결, 토픽 구독신청
4. 토픽 수신대기 , 처리



#### 클라이언트 클래스 인스턴스화 하기

생성자 생략시 디폴트로 지정



비동기로 동작



### 네트워크 루프(프로그래밍)

- loop()

  - 1개의 네트워크 이벤트 처리

- loop_start()

  - 비동기 방식
  - 새로운 스레드를 실행하여 loop()를 무한 실행

- loop_forever()

  - 동기 방식

  - 내부에서 무한루프

  - loop() 무한 실행
  
  - queue작업을 실행
  
    

### 토픽 발간하기 : publish()





### 콜백

- 특정 이벤트(접속 성공, 메시지 수신등) 가 발생했을때 호출되는 핸들러(함수)

- 일반적으로 두 가지 운영
  - 접속 결과 콜백
  - 메시지 수신 콜백

#### on_connect()

rc = result code

rc 값 0,1,2

0 : 연결성공

2 : ip 문제

- broker 주소 지정 문제	// 가장 많이 하는 실수
- conf 문제
- 방화벽 문제
- 서비스 중단된 경우



#### on_message(client,userdata,message)

- client
- **message**
  - MQTTMessage 인스턴스
  - 속성 : topic, payload, qos, retain 
    - topic : 문자열
    - payload : 값, byte 배열
      - byte배열 --------> 문자열 : decode()
      - 문자열 --------> byte배열 : encode()




