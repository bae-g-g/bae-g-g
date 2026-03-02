


![header](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=180&section=header&text=🚙%Gyoung-geun%20Bae%20🤖&fontSize=40)

👋 Hi, I'm Gyoung-geun

🎓 Inchon National University, Embedded Systems Engineering   

🔧 Experienced in Embedded Systems( IoT, mobility,AI Vision projects...)


---

<br>

## 🔧 Tech
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>

![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white) 
![NVIDIA Jetson](https://img.shields.io/badge/NVIDIA%20Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white)


---

### 📊 BOJ Stats

[![Solved.ac 프로필](http://mazassumnida.wtf/api/v2/generate_badge?boj=rudrmsrns)](https://solved.ac/rudrmsrns)


<br>

---
# 📑 Summary of Activities


### [**공장 시스템 자동화 프로젝트 ( 2026.01 ~ 2026.02) - 프로젝트 바로가기**](https://github.com/bae-g-g/smart-logistics-system)
  <details>
    <summary>👉  ( 클릭해서 펼치기 )  공장 물류시스템 (클라우드-엣지-엔드 디바이스) 자동화 시스템 - 삼성 SW 청년 아카데미 프로젝트 우수상</summary>
  
  - **역할:** 시스템 아키텍처 설계, 통신 인프라 구축, 컨베이어 제어 로직 
  - **내용:**
    
    - **아키텍처 설계** : 3계층 폐쇄망 아키텍처 설계 (Cloud ↔ Edge ↔ End-device). VPN 가상망과 로컬 LAN을 동시 운용하는Sidecar Gateway 패턴 적용  
    - **시스템 보안** : 외부망(Cloud↔Edge)mTLS 상호 인증 + 내부망(Edge↔Device) ID/PW 인증 적용, VPN 기반 폐쇄망 구축
    - **미디어 스트리밍** RPi 중계 서버 기반 영상 파이프라인 구축: Jetson →{MPEG-TS/UDP}→ RPi →{WebRTC}→ Web. Nginx 리버스 프록시로 WHEP 세션 처리
    - **DevOps** : Tailscale 컨테이너를 Gateway Router로 사용하는 Sidecar 패턴 Docker Compose 오케스트레이션. 듀얼스택(VPN+LAN) 라우팅 스크립트 작성
    - **Edge 미들웨어** :로컬 MQTT 브로커 + 서버 MQTT 클라이언트 이중 구조의 게이트웨이 통신 모듈 개발. 팩토리 상태 머신 기반 공정 제어 로직 구현
    
    ### Embedded & Hardware
    
    ![Raspberry Pi](https://img.shields.io/badge/-RaspberryPi-C51A4A?style=for-the-badge&logo=Raspberry-Pi)  ![Jetson Nano](https://img.shields.io/badge/NVIDIA%20Jetson-76B900?style=for-the-badge&logo=nvidia&logoColor=white) ![ROS2](https://img.shields.io/badge/ROS2-22314E?style=for-the-badge&logo=ros&logoColor=white)
    
    ### Infrastructure & DevOps
    
    ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) ![Tailscale](https://img.shields.io/badge/Tailscale-18181B?style=for-the-badge&logo=tailscale&logoColor=white) ![OpenSSL](https://img.shields.io/badge/OpenSSL-721412?style=for-the-badge&logo=openssl&logoColor=white) ![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
    
    ### Communication
    
    ![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white) ![GStreamer](https://img.shields.io/badge/GStreamer-73C92D?style=for-the-badge&logo=gstreamer&logoColor=white) ![MPEG-TS](https://img.shields.io/badge/MPEG--TS-000000?style=for-the-badge&logo=ffmpeg&logoColor=white)  ![WebRTC](https://img.shields.io/badge/WebRTC-333333?style=for-the-badge&logo=webrtc&logoColor=white)

  
  </details>
  
  ![시연이미지](https://github.com/bae-g-g/smart-logistics-system/blob/main/img/%EC%A3%BC%EC%B0%A8.gif)


### [**비전인식 델타로봇 프로젝트 ( 2024.09 ~ 2025.06) - 프로젝트 바로가기**](https://github.com/bae-g-g/Vision-PickPlace-DeltaRobot) 
  
  <details>
    <summary>👉 ( 클릭해서 펼치기 ) 비전 인식기반 쓰레기 분류 자동화 델타로봇   - 임베디드 시스템 공학과 캡스톤 프로젝트</summary>
    
    
    
  - **역할:**  : 델타로봇 제어 및 통신 인터페이스 구현 (역기구학, 펌웨어 및 통신 인터페이스) 
  - **내용:**
    - **역기구학 계산** : 델타 로봇의 End-Effector를 원하는 좌표 (x, y, z)로 이동시키기 위해 각 모터의 회전 각도 (theta1,2,3)를 계산하는 핵심 알고리즘 적용.
    - **펌웨어 개발** : TaskScheduler를 통한 모터 병렬제어 및 외부센서를 통한 인텁트 처리
    - **통신 인터페이스 구축** : 젯슨보드와 teensy4.1보드간의 시리얼 통신을 위한 통신 인터페이스 구축

  ### 💻 Languages
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) 
### 🛠 Embedded & Hardware
 ![Teensy 4.1](https://img.shields.io/badge/Teensy%204.1-175596?style=for-the-badge&logo=arduino&logoColor=white) ![Arduino IDE](https://img.shields.io/badge/Arduino_IDE-00979D?style=for-the-badge&logo=arduino&logoColor=white) ![PlatformIO](https://img.shields.io/badge/PlatformIO-F5822A?style=for-the-badge&logo=platformio&logoColor=white) ![NVIDIA Jetson Xavier NX](https://img.shields.io/badge/NVIDIA%20Jetson-76B900?style=for-the-badge&logo=nvidia&logoColor=white)

### 👁️ AI & Computer Vision
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white) ![YOLO](https://img.shields.io/badge/YOLO-00FFFF?style=for-the-badge&logo=yolo&logoColor=black)

  </details>

  ![시연이미지](https://github.com/bae-g-g/Vision-PickPlace-DeltaRobot/blob/main/img/%EC%A0%84%EC%B2%B4%EC%8B%9C%EC%97%B0.gif)

### [**C언어 멘토링 및 학습자료 - 정리문서 바로가기**](https://github.com/bae-g-g/C-study)

- 2023.03 ~ 2025.03 멘토링 자체제작 학습자료
  
