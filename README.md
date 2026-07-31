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

## [Jetson Nano I2C Multi-Device Kernel Driver](https://github.com/clanadian/jetson-i2c-drivers)

Jetson Nano에서 MPU6050·EEPROM·OLED용 Linux I2C 캐릭터 디바이스 드라이버를 구현했습니다.

* Device Tree Overlay 및 probe/remove 기반 드라이버 생명주기 구성
* EEPROM을 활용한 센서 캘리브레이션 데이터 영속 저장
* Tegra I2C Zero-length Write 제약 분석 및 우회 처리

`Linux Kernel` `I2C` `Device Tree` `ioctl`

## [Raspberry Pi 4 FPGA SPI Custom Driver](https://github.com/clanadian/rpi4-spi-driver)

Raspberry Pi 4와 AES-128 FPGA 모듈을 연결하는 커스텀 SPI 커널 드라이버를 구현했습니다.

* spidev 기반 통신 검증 후 커스텀 SPI 드라이버로 전환
* ioctl 기반 Full-Duplex 송수신 인터페이스 설계
* Linux와 FPGA 간 하드웨어·소프트웨어 통합 검증

`Linux Kernel` `SPI` `FPGA` `ioctl`

## [STM32 CAN Gateway & UDS](https://github.com/clanadian/stm32-can-gateway-cluster)

FreeRTOS 기반 다중 ECU CAN 네트워크와 Central Gateway를 구현했습니다.

* ECU 간 CAN 메시지 라우팅 및 통합 제어
* VW Golf Mk6 계기판 CAN 프로토콜 분석
* ISO 14229 기반 UDS 진단 통신 구현

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

# 📫 Contact

📧 woo.yunji2000@gmail.com
