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

## [KR260 ADAS HW–SW Integration Platform](https://github.com/clanadian/kr260-adas-platform) (개발중)

AMD Kria KR260(Zynq UltraScale+ MPSoC)에서 카메라 입력부터 FPGA 기반 YOLO 추론과
UART 안전 상태 출력까지 연결하는 Embedded Linux ADAS 플랫폼입니다.

**담당: PS(APU/RPU) 소프트웨어 및 HW–SW 시스템 통합**

- 카메라 입력·전처리 및 YOLO raw head decode 구현
- 골든 벡터 기반 PL–PS 인터페이스 검증 체계 구축
- AXI4-Lite 레지스터 맵과 HLS DDR 접근 구조 분석 및 인터페이스 계약 정의
- RPU 안전 상태 UART 인터페이스(`CLEAR`/`SLOW`/`STOP`) 설계와 검증 vector 제공
- 실보드 수령 후 PetaLinux bring-up, Device Tree, PL–PS end-to-end 검증 예정

`C++` `V4L2` `Zynq UltraScale+ MPSoC` `AXI4-Lite` `RPU` `PetaLinux 예정` `Device Tree 예정`

---

## [STM32 CAN Gateway & UDS](https://github.com/clanadian/stm32-can-gateway-cluster)

FreeRTOS 기반 다중 ECU CAN gateway와 UDS 진단 통신을 구현했습니다.

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
