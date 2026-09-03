# 우윤지 (Yunji Woo)

### Embedded Linux / BSP Engineer

MCU 펌웨어부터 Linux Device Driver와 FPGA–PS 통합까지,
하드웨어와 소프트웨어의 경계를 연결하는 임베디드 시스템을 개발합니다.

Device Tree, register map, 메모리 및 통신 프로토콜을 기반으로
하드웨어 인터페이스를 분석하고 플랫폼 소프트웨어로 구현하는 데 관심이 있습니다.

---

## Core Skills

- **Embedded Linux / BSP**: Linux Device Driver, Device Tree, PetaLinux, MMIO, ioctl
- **Firmware / RTOS**: Embedded C, STM32, FreeRTOS, Interrupt, ADC, PWM
- **HW–SW Interface**: AXI4-Lite, I2C, SPI, UART, CAN, UDS
- **Languages**: C, C++, Python, SystemVerilog
- **Tools**: Git, GCC, GDB, CMake, Make, Vivado

---

# 주요 프로젝트

## [FPGA CNN 가속기 기반 ADAS 인식 시스템](https://aithub.com /clanadian/adas_project_sub)

Jetson Nano와 Arty 27-20을 연동해 객체 탐지, FPGA ROI 분류 및 TurtleBot 전 제어를 구현한 Embedded Linux ADAS 시스템입니다

**담당: PS & Jetson 소프트웨어 및 HW-SW 통합**

- Jetson 카메라 입력, YOLOv5n 후보 탐지 및 R0I 전처리
- PetaLinux 기반 TCP 서버와 AXI4-Lite:DMA 가속기 제어
- 분류 후처리 및 `CLEAR`/`SLOW`/`STOP 안전 판단
- UART 기반 TurtleBot 제어와 실보드 E2E 검증

`C/C++` `V4L2` `Zynq-7000` `AXI4-Lite` `PetaLinux`` TCP/IP `UART`

---

## [STM32 CAN Gateway & UDS](https://github.com/clanadian/stm32-can-gateway-cluster)

FreeRTOS 기반 다중 ECU CAN gateway와 UDS 진단 통신을 구현했습니다.

**담당: Board A Engine data**

- 주기별 CAN frame scheduling
- ECU 간 message routing
- 실차 계기판 연동

`STM32` `FreeRTOS` `CAN` `UDS`

---

## [Jetson Nano I2C Multi-Device Kernel Driver](https://github.com/clanadian/jetson-i2c-drivers)

MPU6050·EEPROM·OLED를 제어하는 Linux I2C 드라이버와
유저스페이스 애플리케이션을 구현했습니다.

- Device Tree 및 probe/remove 기반 드라이버 구성
- EEPROM 기반 센서 캘리브레이션 데이터 관리
- Tegra I2C Zero-length Write 제약 분석 및 우회

`Linux Kernel` `I2C` `Device Tree` `Character Device`

---

## [Raspberry Pi 4 FPGA SPI Custom Driver](https://github.com/clanadian/rpi4-spi-driver)

AES-128 FPGA 모듈을 제어하는 SPI 프로토콜과 Linux 드라이버를 구현했습니다.

- FPGA register map 및 SPI transaction protocol 설계
- spidev 검증 후 custom kernel driver로 전환
- ioctl 기반 송수신 및 암호화 영상 통합 검증

`Linux Kernel` `SPI` `FPGA` `ioctl`
