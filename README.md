# 우윤지 (Yunji Woo)

### Embedded Linux · BSP · Device Driver Engineer

하드웨어와 운영체제를 연결하는 소프트웨어를 개발합니다.

레지스터 레벨 제어부터 Linux 커널 드라이버, Device Tree, BSP까지
하드웨어가 운영체제 위에서 정상적으로 동작하기 위한 소프트웨어 계층에 관심이 있습니다.

---

# 🛠 Tech Stack

### Language
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Verilog](https://img.shields.io/badge/Verilog-005B99?style=flat-square)

### Embedded / OS
![Linux Kernel](https://img.shields.io/badge/Linux%20Kernel-FCC624?style=flat-square&logo=linux&logoColor=black)
![FreeRTOS](https://img.shields.io/badge/FreeRTOS-000000?style=flat-square)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![Jetson Nano](https://img.shields.io/badge/Jetson%20Nano-76B900?style=flat-square&logo=nvidia&logoColor=white)
### Interface / Protocol

`I2C` `SPI` `UART` `CAN` `Device Tree` `ioctl`

### Tools
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Vivado](https://img.shields.io/badge/Vivado-orange?style=flat-square)

---

# 🚀 주요 프로젝트

## [Jetson Nano I2C Multi-Device Kernel Driver](https://github.com/clanadian/jetson-i2c-drivers.git)

Jetson Nano(Linux 4.9 L4T) 환경에서 MPU6050, EEPROM, OLED용
Linux 캐릭터 디바이스 드라이버를 직접 구현했습니다.

- Device Tree Overlay 등록
- probe/remove 기반 Driver Lifecycle 관리
- EEPROM 기반 센서 캘리브레이션
- Tegra I2C Zero-length Write 제약 분석 및 해결

**Tech**

`Linux Kernel` `I2C` `Device Tree` `ioctl`

---

## [Raspberry Pi4 - FPGA SPI Custom Driver](https://github.com/clanadian/rpi4-spi-driver.git)

FPGA(AES-128)와 Raspberry Pi를 SPI로 연결하는
커스텀 Linux 커널 드라이버를 구현했습니다.

- spidev 프로토타입 구현
- Custom SPI Driver 전환
- ioctl 기반 Full-Duplex 인터페이스 설계
- FPGA와 Linux 간 HW/SW 연동

**Tech**

`SPI` `Linux Kernel` `FPGA`

---

## [STM32 CAN Gateway & UDS](https://github.com/clanadian/stm32-can-gateway-cluster.git)

FreeRTOS 기반 차량 CAN 네트워크와
Central Gateway를 구현했습니다.

- Multi ECU CAN Network
- Gateway Routing
- VW Golf Mk6 계기판 Reverse Engineering
- ISO 14229 UDS 진단 통신 구현

**Tech**

`STM32` `FreeRTOS` `CAN` `UDS`

---

# 🔭 진행 중인 프로젝트

### KR260 Embedded AI Platform

Xilinx Kria KR260 기반 Embedded Linux 플랫폼을 개발하고 있습니다.

- PetaLinux BSP
- Device Tree
- DPU 기반 CNN 추론
- ROS2 연동
- HW/SW Co-design

---

# 📌 Pinned Repository

아래 저장소에서 다음 프로젝트를 확인할 수 있습니다.

- Linux Kernel Driver
- Embedded Linux / BSP
- FPGA HW/SW Co-design
- STM32 Embedded System
- Automotive CAN

👇 Pinned Repository를 확인해주세요.

---

# 📫 Contact

📧 woo.yunji2000@gmail.com
