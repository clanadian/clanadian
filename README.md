# 우윤지 (Yunji Woo)

### Embedded Software Engineer

MCU 펌웨어부터 Linux 커널 드라이버까지  
하드웨어를 제어하는 임베디드 소프트웨어를 개발합니다.

STM32·FreeRTOS 기반 제어 및 통신 시스템과  
Linux Device Driver·Device Tree 기반 하드웨어 연동을 경험했습니다.

하드웨어의 동작 원리와 통신 프로토콜을 이해하고,  
플랫폼 환경에 맞는 소프트웨어 계층을 설계하는 데 관심이 있습니다.

---

# 🛠 Tech Stack

### Language

![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Verilog](https://img.shields.io/badge/Verilog-005B99?style=flat-square)

### Firmware / Embedded

![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![FreeRTOS](https://img.shields.io/badge/FreeRTOS-000000?style=flat-square)

`Embedded C` `STM32 HAL` `FreeRTOS` `ADC` `PWM` `Interrupt`

### Embedded Linux

![Linux Kernel](https://img.shields.io/badge/Linux%20Kernel-FCC624?style=flat-square&logo=linux&logoColor=black)
![Jetson Nano](https://img.shields.io/badge/Jetson%20Nano-76B900?style=flat-square&logo=nvidia&logoColor=white)

`Linux Device Driver` `Character Device` `Device Tree` `ioctl`

### Interface / Protocol

`I2C` `SPI` `UART` `CAN` `UDS` `Bluetooth`

### Tools

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Vivado](https://img.shields.io/badge/Vivado-orange?style=flat-square)

`GCC` `GDB` `Make` `PetaLinux`

---

# 🚀 주요 프로젝트

## [STM32 CAN Gateway & UDS](https://github.com/clanadian/stm32-can-gateway-cluster)

STM32와 FreeRTOS를 기반으로 다중 ECU 차량 네트워크와  
실차 계기판 연동 시스템을 구현했습니다.

- ADC 입력을 기반으로 RPM·Speed·Coolant 차량 데이터 생성
- FreeRTOS 태스크 기반 50ms·100ms·1000ms CAN 프레임 스케줄링
- ECU 간 CAN 메시지 라우팅 및 Central Gateway 구현
- VW Golf Mk6 계기판 CAN Payload 분석 및 실기기 연동
- ISO 14229 기반 UDS 진단 통신 구현

`Embedded C` `STM32` `FreeRTOS` `CAN` `UDS`

---

## [Jetson Nano I2C Multi-Device Kernel Driver](https://github.com/clanadian/jetson-i2c-drivers)

Jetson Nano에서 MPU6050·EEPROM·OLED용  
Linux I2C 캐릭터 디바이스 드라이버를 구현했습니다.

- Device Tree 기반 디바이스 등록
- probe/remove 기반 드라이버 생명주기 구성
- EEPROM을 활용한 캘리브레이션 데이터 영속 저장
- Tegra I2C Zero-length Write 제약 분석 및 우회
- 커널 드라이버부터 유저스페이스 애플리케이션까지 통합 검증

`Linux Kernel` `I2C` `Device Tree` `Character Device`

---

## [Raspberry Pi 4 FPGA SPI Custom Driver](https://github.com/clanadian/rpi4-spi-driver)

Raspberry Pi 4와 AES-128 FPGA 모듈을 연결하는  
SPI 통신 프로토콜과 커스텀 Linux 드라이버를 구현했습니다.

- FPGA 레지스터 맵 및 SPI 트랜잭션 프로토콜 설계
- spidev 기반 통신 검증 후 커스텀 SPI 드라이버로 전환
- ioctl 기반 Full-Duplex 송수신 인터페이스 구현
- 커널 전송 계층과 유저스페이스 프로토콜 계층 분리
- FPGA 암호화 영상 수신·복호화·출력 전 과정 검증

`Linux Kernel` `SPI` `FPGA` `ioctl` `AES-128`

---

## [FPGA I2C Multi-Slave Door Lock](https://github.com/clanadian)

FPGA에서 I2C Master를 직접 설계하고  
OLED와 EEPROM을 연동한 디지털 도어락을 구현했습니다.

- START·STOP·ACK 처리를 포함한 I2C Master FSM 설계
- OLED와 EEPROM이 공유하는 I2C 버스 중재 로직 구현
- 비밀번호 및 실패 횟수 EEPROM 영속 저장
- SCL 9펄스 기반 I2C Bus Clear 루틴 구현
- 테스트벤치와 실기기를 통한 전체 동작 검증

`SystemVerilog` `FPGA` `I2C` `FSM` `EEPROM`

---

# 🔭 진행 중인 프로젝트

## KR260 Embedded AI Platform

Xilinx Kria KR260 기반 Embedded Linux 및  
온디바이스 AI 실행 환경을 개발하고 있습니다.

- PetaLinux 기반 시스템 이미지 구성
- Device Tree 및 주변장치 인터페이스 설정
- C++ 기반 영상 전처리·추론 파이프라인 개발
- DPU 기반 CNN 추론
- ROS2 시스템 연동
- FPGA 가속기와 소프트웨어 간 인터페이스 설계

---

# 📫 Contact

📧 woo.yunji2000@gmail.com
