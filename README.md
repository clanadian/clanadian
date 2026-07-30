# 우윤지 (Yunji Woo)
### Embedded Linux · BSP · Device Driver Engineer

하드웨어가 운영체제 위에서 실제로 동작하게 만드는 소프트웨어 계층을 만듭니다.
레지스터 맵 설계부터 Linux 커널 드라이버 구현까지, 하드웨어와 OS의 경계에서 일하는 걸 좋아합니다.

---

## 🛠 Tech Stack

**Language**
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Verilog](https://img.shields.io/badge/Verilog-005B99?style=flat-square)

**OS / Platform**
![Linux Kernel](https://img.shields.io/badge/Linux%20Kernel-FCC624?style=flat-square&logo=linux&logoColor=black)
![FreeRTOS](https://img.shields.io/badge/FreeRTOS-000000?style=flat-square)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![Jetson Nano](https://img.shields.io/badge/Jetson%20Nano-76B900?style=flat-square&logo=nvidia&logoColor=white)

**Interface / Protocol**
`I2C` `SPI` `UART` `CAN` `Device Tree` `ioctl`

**Tools**
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Vivado](https://img.shields.io/badge/Vivado-orange?style=flat-square)

---

## 🚀 Featured Projects

### [Jetson Nano I2C Multi-Device Kernel Driver](https://github.com/YOUR_ID/REPO_NAME)
Linux 4.9(L4T) 환경에서 MPU6050 · EEPROM · OLED용 캐릭터 디바이스 드라이버 직접 구현.
Device Tree Overlay 등록, probe 기반 lifecycle 관리, Tegra I2C 하드웨어 제약(zero-length write 미지원) 분석 및 해결.

### [RPi4–FPGA SPI Custom Kernel Driver (AES-128)](https://github.com/YOUR_ID/REPO_NAME)
FPGA가 AES-128로 암호화해 전송한 영상 데이터를 SPI로 수신하는 커스텀 커널 드라이버 구현.
spidev 기반 프로토타입 → 커스텀 드라이버 구조로 전환, ioctl 기반 풀듀플렉스 전송 인터페이스 설계.

### [STM32 기반 차량 CAN 통신 & 계기판 연동](https://github.com/YOUR_ID/REPO_NAME)
FreeRTOS 기반 다중 ECU · Central Gateway 네트워크 구현. 실차(VW Golf Mk6) 계기판 CAN Payload 리버싱 및 UDS 진단 통신 End-to-End 검증.

더 많은 프로젝트는 아래 Pinned Repositories 참고 👇

---

## 🔭 Currently Building
Xilinx Kria KR260 (Zynq UltraScale+ MPSoC) 기반 PetaLinux 커스텀 BSP + DPU 기반 CNN 추론 + ROS2 로봇 연동 프로젝트 진행 중

---

## 📊 GitHub Stats

![Yunji's GitHub stats](https://github-readme-stats.vercel.app/api?username=YOUR_ID&show_icons=true&theme=default&hide_border=true)

---

## 📫 Contact
- Email: woo.yunji2000@gmail.com
