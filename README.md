# Node-Red  
### Node-RED란?  
- IoT 연결을 시각화 도구로 연결 가능한 개발 도구
- IBM의 Emerging Technology Service 팀이 개발한 flow 기반 프로그래밍 도구
- JSON을 사용하여 저장
- Node.js 위에서 개발됨
- 장점
  - 복합한 TLS 인증을 쉽게 사용할 수 있다.
  - GUI 방식으로 코드 없이 쉽게 제작이 가능하다.
  - Web/Mobile에서 접속 가능한 시각화 앱을 쉽게 제작이 가능하다.

#### 설치 및 실행
1. https://nodejs.org/en 에서 LTS 버전 설치
2. cmd 창에서 설치 명령어를 입력한다.
   - npm install -g node-red (-g : 글로벌 설치 옵션)
3. cmd 창에서 node-red 실행 한 후
   - chrome을 켜고 “127.0.0.1:1880” 을 입력한다.

### Node-RED MQTT  
config 파일의 설정대로 Rpi5 MQTT Broker 서버를 재실행한다.  
```
• cd /etc/mosquitto
• sudo /etc/init.d/mosquitto stop
• sudo mosquitto –c mosquitto.conf –v
```
#### Rpi5 MQTT subscribe  
![mqtt(in) - debug](https://github.com/kghees/Node-Red/assets/92205960/847e6a90-b632-4a31-a3cb-b242e8066866)  
![mqtt-rasberripi 설정2](https://github.com/kghees/Node-Red/assets/92205960/d2ae0074-352c-44d0-a2c9-ed376f33f650)
![mqtt input 결과](https://github.com/kghees/Node-Red/assets/92205960/af7cec8f-b03f-4ecf-80bc-40d88277664e)  

#### Rpi5 MQTT publish  
![mqtt ouput 결과](https://github.com/kghees/Node-Red/assets/92205960/dbd7409a-5a74-4287-8800-a0ecbb7e5445)  

####  센서 노드 연결하기  
![esp32 통신 결과](https://github.com/kghees/Node-Red/assets/92205960/c8fbe284-1086-4363-a1fe-dab6538bb89a)  

### Node-RED MQTT - AWS  
![image](https://github.com/kghees/Node-Red/assets/92205960/befc74cb-fb77-4a73-af2b-9856692bf7bb)  
![AWS-mqtt(in,out)](https://github.com/kghees/Node-Red/assets/92205960/12e1336c-5935-4f21-a212-b4411f594228)
![AWS-mqtt 결과](https://github.com/kghees/Node-Red/assets/92205960/cd43f425-9006-4588-bbea-1ba5c970306f)  
![AWS-mqtt publish 결과](https://github.com/kghees/Node-Red/assets/92205960/40e05275-2cc0-4001-b0ba-1359e169098b)

### IoT 시스템  

![image](https://github.com/kghees/Node-Red/assets/92205960/85ab7519-3a78-431c-bb70-d9ca9b0f147e)
![AWS-esp32-rasberripi 결과2](https://github.com/kghees/Node-Red/assets/92205960/81419678-0275-4a64-b9b8-cb69f79dab5b)  
![AWS-esp32-rasberripi 결과](https://github.com/kghees/Node-Red/assets/92205960/773151fc-6d13-43bc-966f-c606e53f868a)







