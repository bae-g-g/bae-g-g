


![header](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=180&section=header&text=🚙%Gyoung-geun%20Bae%20🤖&fontSize=40)

👋 Hi, I'm Gyoung-geun Bae

🎓 Incheon National University, Embedded Systems Engineering / Samsung SW·AI Academy For Youth(SSAFY)

🔧 I build embedded/robotics systems across firmware, edge AI, communication, and control.

🚀 Main interests: Network · Robotics · Embedded Linux · Computer Vision · Edge AI · System Integration


---

<br>

## 🔧 Tech

### Languages

![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

### Embedded / Robotics

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white) 
![NVIDIA Jetson](https://img.shields.io/badge/NVIDIA%20Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white)

### Vision / AI

![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![YOLO](https://img.shields.io/badge/YOLO-00FFFF?style=flat-square&logo=yolo&logoColor=black)

### Communication / Infra


![UDP](https://img.shields.io/badge/UDP-000000?style=flat-square&logo=socketdotio&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white)
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
![UART](https://img.shields.io/badge/UART-555555?style=flat-square&logo=serialport&logoColor=white)
![I2C](https://img.shields.io/badge/I2C-555555?style=flat-square&logo=stmicroelectronics&logoColor=white)


---


## 🏆 Awards

- **삼성 소프트웨어 역량 테스트(26.03) - B형 취득**
- **[SSAFY 프로젝트 전시발표회](https://github.com/jeayoungho97/SPOT_GET_IT)(26.06) - 전국 캠퍼스 1위**
- **SSAFY 자율주행 시뮬레이션 프로젝트(26.03) - 우수상**
- **[SSAFY AIOT 프로젝트](https://github.com/bae-g-g/smart-logistics-system)(26.02) - 우수상**
- **[인천대 진로 및 전공박람회](https://github.com/bae-g-g/Vision-PickPlace-DeltaRobot)(25.05)  - 임베디드시스템과 대표 전시작품 선정** 
- **9회 INU 메이커 경진대회(24.12) - 장려**
- **미래모빌리티 첨단 융합 설계(24.08) - 금상**
- **7회 INU 메이커 경진대회(22.12) - 우수상**

<br>

---

## 🔎 Project Focus

| Project | My Role | Keywords |
| --- | --- | --- |
| 다중 정찰 로봇 및 관제 프로젝트 | RPi5 브릿지 앱, UDP 패킷 재조립, POSIX 공유메모리, Qt6 관제 연동 | UDP, POSIX SHM, Qt6, Multi-robot Monitoring |
| Smart Logistics System | 3계층 폐쇄망 아키텍처, MQTT 게이트웨이, 영상 스트리밍, 컨베이어 제어 | Tailscale, Docker, mTLS, MQTT, WebRTC |
| Vision-PickPlace-DeltaRobot | 델타로봇 역기구학, Teensy 펌웨어, Jetson-MCU Serial 통신 | Inverse Kinematics, Firmware, Serial, Stepper Motor |
| 리인 트레이싱 RC Car | OpenCV 라인트레이싱, Raspberry Pi-Arduino Serial 통신, Flask 관제 스트리밍 | OpenCV, Serial, MJPEG, Autonomous Driving |
| C Mentoring | C 언어/Arduino 기초 학습자료 제작 및 멘토링 | C, Arduino, Teaching, Documentation |

<br>

---
# 📑 Summary of Activities



### [**다중 정찰 로봇 및 관제 프로젝트 (2026.04 ~ 2026.05[8주]) - 프로젝트 바로가기**](https://github.com/jeayoungho97/SPOT_GET_IT)
<details>
  <summary>👉( 클릭해서 펼치기 )  마이크로 스팟 기반 4족 보행 로봇 및 다중 로봇을 이용한 정찰/관제 시스템 - 삼성 SW 청년 아카데미 프로젝트 전시발표회 전국 1위 </summary>

- **역할:** RPi5 브릿지 앱 구현, Jetson-RPi UDP 통신, POSIX 공유메모리 기반 Qt 대시보드 연동
- **내용:**
  - **UDP 통신 브릿지 구현** : Jetson 로봇에서 송신하는 이미지, LiDAR, 오도메트리, 상태, 이벤트, 경로 데이터를 RPi5 브릿지 데몬에서 수신하는 통신 구조 구현.
  - **분할 패킷 재조립** : UDP로 분할 전송되는 이미지/LiDAR 데이터를 재조립하고, Qt 대시보드가 읽을 수 있는 형태로 공유메모리에 기록.
  - **POSIX 공유메모리 IPC 설계** : 브릿지 데몬과 Qt6 대시보드 사이를 POSIX shared memory, semaphore, atomic 필드 기반으로 연결해 센서 데이터와 상태 정보를 분리 관리.
  - **다중 로봇 관제 구조** : `/robot_bridge_0`, `/robot_bridge_1` 형태의 로봇별 공유메모리 구조를 사용해 다중 로봇 모니터링 확장성을 고려.
  - **제어 명령 송신 흐름** : Qt에서 생성한 이동/정지/비상정지/미션 명령을 공유메모리 `cmd_queue`에 기록하고, 브릿지 데몬이 Jetson으로 송신하는 명령 흐름 구성.

### 💻 Languages

![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)

### 🛠 Embedded & Robotics

![Raspberry Pi 5](https://img.shields.io/badge/Raspberry%20Pi%205-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white) ![Jetson Orin Nano](https://img.shields.io/badge/NVIDIA%20Jetson%20Orin%20Nano-76B900?style=for-the-badge&logo=nvidia&logoColor=white)

### 🔗 Communication & IPC

![UDP](https://img.shields.io/badge/UDP-000000?style=for-the-badge&logo=socketdotio&logoColor=white) ![POSIX SHM](https://img.shields.io/badge/POSIX%20SHM-555555?style=for-the-badge&logo=linux&logoColor=white) ![Qt6](https://img.shields.io/badge/Qt6-41CD52?style=for-the-badge&logo=qt&logoColor=white) !

</details>

<img width="400" height="308" alt="spotgetit" src="https://github.com/user-attachments/assets/998d2423-0931-49d2-9808-3b84a801560a" />



### [**공장 시스템 자동화 프로젝트 ( 2026.01 ~ 2026.02[7주]) - 프로젝트 바로가기**](https://github.com/bae-g-g/smart-logistics-system)
  <details>
    <summary>👉  ( 클릭해서 펼치기 )  공장 물류시스템 (클라우드-엣지-엔드 디바이스) 자동화 시스템 - 삼성 SW 청년 아카데미 프로젝트 우수상</summary>
  
  - **역할:** Cloud-Edge-End-device 아키텍처 설계, 통신 인프라/보안 구성, Edge 미들웨어 및 컨베이어 제어 구현
  - **내용:**
    
    - **아키텍처 설계** : Cloud ↔ Edge ↔ End-device 3계층 구조 설계. VPN 가상망과 로컬 LAN을 함께 운용하는 Sidecar Gateway 패턴 적용.
    - **시스템 보안** : Cloud-Edge 구간 mTLS 상호 인증, Edge-Device 구간 ID/PW 인증 적용. 외부 포트 노출을 줄이는 VPN 기반 폐쇄망 구성.
    - **미디어 스트리밍** : Jetson → MPEG-TS/UDP → RPi → WebRTC/WHEP → Web 흐름의 영상 중계 파이프라인 구축. Nginx 리버스 프록시로 WHEP 세션 처리.
    - **DevOps/네트워크** : Tailscale 컨테이너를 Gateway Router로 활용하는 Docker Compose 구성. VPN/LAN 듀얼스택 라우팅 스크립트 작성.
    - **Edge 미들웨어** : 로컬 MQTT 브로커와 서버 MQTT 클라이언트를 분리한 게이트웨이 통신 모듈 개발. 팩토리 상태 머신 기반 공정 제어 로직 구현.
    - **컨베이어 제어** : Raspberry Pi GPIO/I2C 기반 DC 모터, 서보모터, IR 센서, 상태 LED 제어 흐름 구현.
    
    ### Embedded & Hardware
    
    ![Raspberry Pi](https://img.shields.io/badge/-RaspberryPi-C51A4A?style=for-the-badge&logo=Raspberry-Pi)  ![Jetson Nano](https://img.shields.io/badge/NVIDIA%20Jetson-76B900?style=for-the-badge&logo=nvidia&logoColor=white)
    
    ### Infrastructure & DevOps
    
    ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) ![Tailscale](https://img.shields.io/badge/Tailscale-18181B?style=for-the-badge&logo=tailscale&logoColor=white) ![OpenSSL](https://img.shields.io/badge/OpenSSL-721412?style=for-the-badge&logo=openssl&logoColor=white) ![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
    
    ### Communication
    
    ![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white) ![GStreamer](https://img.shields.io/badge/GStreamer-73C92D?style=for-the-badge&logo=gstreamer&logoColor=white) ![MPEG-TS](https://img.shields.io/badge/MPEG--TS-000000?style=for-the-badge&logo=ffmpeg&logoColor=white)  ![WebRTC](https://img.shields.io/badge/WebRTC-333333?style=for-the-badge&logo=webrtc&logoColor=white)

  
  </details>
  
  ![시연이미지](https://github.com/bae-g-g/smart-logistics-system/blob/main/img/%EC%A3%BC%EC%B0%A8.gif)






### [**비전인식 델타로봇 프로젝트 ( 2024.09 ~ 2025.06) - 프로젝트 바로가기**](https://github.com/bae-g-g/Vision-PickPlace-DeltaRobot) 
  
  <details>
    <summary>👉 ( 클릭해서 펼치기 ) 비전 인식기반 쓰레기 분류 자동화 델타로봇   - 임베디드 시스템 공학과 캡스톤 프로젝트</summary>
    
    
    
  - **역할:** 델타로봇 제어 및 통신 인터페이스 구현 (역기구학, 펌웨어 및 통신 인터페이스) 
  - **내용:**
    - **역기구학 계산** : 델타 로봇의 End-Effector 목표 좌표 (x, y, z)를 3축 모터 각도(theta1, theta2, theta3)로 변환하는 제어 로직 구현.
    - **펌웨어 개발** : Teensy 4.1 기반 스텝 모터 제어 펌웨어 구현. TaskScheduler와 인터럽트를 활용해 데이터 수신과 모터 제어 흐름을 분리.
    - **통신 인터페이스 구축** : Jetson Xavier NX의 상위 제어 코드와 Teensy 펌웨어 사이의 Serial 통신 인터페이스 구현.
    - **시스템 통합** : 카메라 인식 결과가 실제 로봇의 픽앤플레이스 동작으로 이어지도록 인식-좌표 변환-모터 제어 파이프라인 연동.

  ### 💻 Languages
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) 
### 🛠 Embedded & Hardware
 ![Teensy 4.1](https://img.shields.io/badge/Teensy%204.1-175596?style=for-the-badge&logo=arduino&logoColor=white) ![Arduino IDE](https://img.shields.io/badge/Arduino_IDE-00979D?style=for-the-badge&logo=arduino&logoColor=white) ![PlatformIO](https://img.shields.io/badge/PlatformIO-F5822A?style=for-the-badge&logo=platformio&logoColor=white) ![NVIDIA Jetson Xavier NX](https://img.shields.io/badge/NVIDIA%20Jetson-76B900?style=for-the-badge&logo=nvidia&logoColor=white)

  </details>

  ![시연이미지](https://github.com/bae-g-g/Vision-PickPlace-DeltaRobot/blob/main/img/%EC%A0%84%EC%B2%B4%EC%8B%9C%EC%97%B0.gif)

### [**C언어 멘토링 및 학습자료 - 정리문서 바로가기**](https://github.com/bae-g-g/C-study)

- **기간:** 2023.03 ~ 2025.03
- **내용:** C 언어 기초, 포인터, 배열, 구조체, Arduino 입문 내용을 직접 학습자료로 정리하고 멘토링 진행
- **의미:** 단순 사용 경험을 넘어, 다른 사람이 이해할 수 있도록 개념을 구조화하고 설명하는 훈련을 지속

### [**RC Car 수동/자동 주행 및 제어 시스템 프로젝트 ( 2025.05 ~ 2025.06 ) - 프로젝트 바로가기**](https://github.com/psy1218/RC_Car)

<details>
    <summary>👉 ( 클릭해서 펼치기 )  비전 인식 라인트레이싱 및 수동 제어 RC카 시스템  (2025.05~2025.06)</summary>

- **역할:** 비전 인식 기반 라인트레이싱 영상 처리, 이기종 간 시리얼 통신 인터페이스 설계, 실시간 웹 스트리밍 환경 구축
- **내용:**
  - **비전 인식 기반 자율 주행 구현** : Raspberry Pi 5 + Picamera2 환경에서 OpenCV 기반 도로 라인 디텍션 적용. 그림자/빛 노이즈 문제를 줄이기 위해 히스토그램 평활화, 모폴로지 Opening, 가우시안 블러, 이진화 전처리 파이프라인 최적화.
  - **시리얼 통신 인터페이스 구축** : 라즈베리파이에서 연산된 조향값(-50~+50 범위의 데이터)을 아두이노 측으로 매 프레임(33.3ms, 9600 baud rate) 지속 전송하는 시리얼 통신 연결 및 포트 예외 복구 로직 구현.
  - **영상 스트리밍 서버 구축** : Flask 기반 원격 관제 웹 서버 구현. MJPEG 스트리밍 방식으로 전방 카메라와 Vision 처리 결과를 브라우저에 송출.
  - **제어 아키텍처 통합** : 수신기(R9DS) 및 조종기(AT9)를 통한 수동/자율주행 모드 전환, ESC/서보모터 제어, 긴급 모듈 사출 기능을 통합 테스트.



### 💻 Languages

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)

### 🛠 Embedded & Hardware

![Raspberry Pi](https://img.shields.io/badge/-RaspberryPi-C51A4A?style=for-the-badge&logo=Raspberry-Pi) ![Arduino UNO](https://img.shields.io/badge/Arduino_UNO-00979D?style=for-the-badge&logo=arduino&logoColor=white)

### 👁️ Computer Vision
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)


</details>



