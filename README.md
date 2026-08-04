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

## [KR260 ADAS HW–SW Integration Platform](KR260_저장소_링크)

Xilinx Kria KR260에서 카메라 입력부터 FPGA 추론 가속기와
TurtleBot 제어까지 연결하는 Embedded Linux 플랫폼을 개발하고 있습니다.

**담당: PS 소프트웨어 및 시스템 통합**

- V4L2 MMAP 기반 카메라 캡처와 멀티스레드 C++ 영상 파이프라인 구현
- RGB UINT8/NCHW 모델 입력과 signed INT8/NHWC HLS 인터페이스 사이의 adapter 설계
- AXI4-Lite register map과 HLS `m_axi` DDR 접근 구조 분석
- PL–PS 인터페이스 계약과 재현 가능한 golden test vector 구성
- YOLO raw head decode/NMS 및 전체 처리 지연 계측
- 변경되는 PL 빌드에 대응하기 위한 Device Tree Overlay 구조 설계
- 향후 RPU 위험 판단 및 ROS2 TurtleBot 제어 시스템 통합

`KR260` `Embedded Linux` `C++` `V4L2` `AXI` `Device Tree` `HLS` `ROS2`

---

## [STM32 CAN Gateway & UDS](링크)

FreeRTOS 기반 다중 ECU CAN gateway와 UDS 진단 통신을 구현했습니다.

- 주기별 CAN frame scheduling
- ECU 간 message routing
- 실차 계기판 연동
- ISO 14229 기반 UDS 구현

`STM32` `FreeRTOS` `CAN` `UDS`

---

## [Jetson Nano I2C Multi-Device Kernel Driver](링크)

MPU6050·EEPROM·OLED를 제어하는 Linux I2C 드라이버와
유저스페이스 애플리케이션을 구현했습니다.

- Device Tree 및 probe/remove 기반 드라이버 구성
- EEPROM 기반 센서 캘리브레이션 데이터 관리
- Tegra I2C Zero-length Write 제약 분석 및 우회

`Linux Kernel` `I2C` `Device Tree` `Character Device`

---

## [Raspberry Pi 4 FPGA SPI Custom Driver](링크)

AES-128 FPGA 모듈을 제어하는 SPI 프로토콜과 Linux 드라이버를 구현했습니다.

- FPGA register map 및 SPI transaction protocol 설계
- spidev 검증 후 custom kernel driver로 전환
- ioctl 기반 송수신 및 암호화 영상 통합 검증

`Linux Kernel` `SPI` `FPGA` `ioctl`

---

## FPGA I2C Multi-Slave Door Lock(https://github.com/clanadian/basys3-i2c-doorlock)

OLED와 EEPROM을 공유하는 I2C Master 및 디지털 도어락을 설계했습니다.

- START·STOP·ACK를 처리하는 I2C Master FSM
- 다중 slave 제어와 bus recovery
- 테스트벤치 및 실기기 검증

`SystemVerilog` `FPGA` `I2C` `FSM`
