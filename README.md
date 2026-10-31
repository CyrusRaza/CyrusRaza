::: {align="center"}
# Hi, I'm Cyrus Naqvi 👋

### Embedded Software Engineer \| Firmware Developer \| IoT & Embedded Linux

**Building reliable firmware and connected embedded systems --- from
microcontrollers to Linux-based gateways.**

📍 Germany · 🎓 MSc Embedded Systems, TU Chemnitz

[![Email](https://img.shields.io/badge/Email-c.razanaqvi%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:c.razanaqvi@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Explore%20my%20work-181717?style=for-the-badge&logo=github)](https://github.com/)
:::

------------------------------------------------------------------------

## 👨‍💻 About Me

I'm an Embedded Software Engineer with an MSc in Embedded Systems from
**TU Chemnitz** and a background in Mechatronics.

My experience spans firmware development in **C**, RTOS-based
concurrency, wireless communication, IoT architectures, and
hardware-level debugging. I developed an ESP32-based LoRaWAN
communication system, including multithreaded firmware, synchronization,
payload fragmentation, and validation on real hardware.

I enjoy working close to the hardware: understanding system constraints,
designing modular firmware, debugging interfaces, and building solutions
that behave reliably outside the development environment.

**Areas I work with:** - Embedded firmware in C and
microcontroller-based systems - RTOS concepts, multithreading, mutexes
and semaphores - IoT connectivity: LoRaWAN, Zigbee, MQTT and WebSocket -
Embedded Linux and Raspberry Pi-based systems - Hardware interfaces,
debugging and system validation - Computer vision and event-camera
research

------------------------------------------------------------------------

## 🛠️ Technical Skills

  -----------------------------------------------------------------------
  Category                            Technologies
  ----------------------------------- -----------------------------------
  **Programming**                     C, C++, Python, MATLAB, VHDL,
                                      Assembly (AVR/ARM)

  **MCUs & Platforms**                ESP32, STM32 (ARM Cortex-M),
                                      MSP430, Raspberry Pi

  **Operating Systems**               FreeRTOS, Zephyr, Bare-metal,
                                      Embedded Linux

  **Wireless & IoT**                  LoRaWAN (EU868), Zigbee, Wi-Fi

  **Communication**                   MQTT, WebSocket

  **Peripherals & Interfaces**        UART, SPI, I²C, PWM, ADC, GPIO,
                                      Timers

  **Concurrency**                     Threads, Mutexes, Semaphores

  **Debugging**                       GDB, JTAG/SWD, Oscilloscope, Logic
                                      Analyzer

  **Build, Test & CI**                CMake, Git, Docker, GitHub Actions,
                                      Unity

  **Computer Vision & ML**            OpenCV, PyTorch, TensorFlow, NumPy,
                                      Event Cameras

  **Other**                           MATLAB/Simulink, AES-128
                                      fundamentals
  -----------------------------------------------------------------------

### Tools & Technologies

::: {align="center"}
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FreeRTOS](https://img.shields.io/badge/FreeRTOS-2C3E50?style=flat-square)
![Zephyr](https://img.shields.io/badge/Zephyr-4B0082?style=flat-square)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)
![Raspberry
Pi](https://img.shields.io/badge/Raspberry_Pi-C51A4A?style=flat-square&logo=raspberrypi&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=flat-square&logo=cmake&logoColor=white)
![GitHub
Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
:::

------------------------------------------------------------------------

## 🚀 Featured Projects

### 1. Embedded Communication Framework --- C

A modular, multithreaded communication pipeline designed to support
multiple transport protocols through a common architecture.

**Highlights** - Runtime protocol selection using the Strategy Pattern
and function pointers - MQTT and WebSocket transport implementations -
Extendable architecture designed to add transports without changing
existing pipeline logic - Unit testing with Unity - CMake build system,
Docker and GitHub Actions CI

**Technologies:** C · Multithreading · MQTT · WebSocket · Unity · CMake
· Docker · GitHub Actions

> **What it demonstrates:** Modular embedded software architecture,
> separation of concerns, testability and CI practices.

**Repository:** Add your project repository link here.

------------------------------------------------------------------------

### 2. LoRaWAN Communication System --- ESP32

Developed firmware for a LoRaWAN communication system as the sole
developer during my work at TU Chemnitz.

**Highlights** - Three-thread firmware architecture: main, send and
receive - Thread safety using mutexes and semaphores - Fragmentation of
222-byte payloads - Operation within EU868 duty-cycle constraints -
24-hour continuous validation on physical hardware - Python server-side
tooling and MQTT forwarding

**Technologies:** C · ESP32 · RTOS · LoRaWAN · MQTT · Python ·
Concurrency

> **What it demonstrates:** Firmware ownership, RTOS concurrency,
> wireless communication constraints and hardware-based validation.

------------------------------------------------------------------------

### 3. IoT Smart Irrigation System

A multi-node IoT architecture connecting sensor nodes, a gateway and an
Embedded Linux platform.

**Highlights** - MSP430-based sensor nodes - STM32 (ARM Cortex-M)
gateway - Raspberry Pi running Embedded Linux - Wireless communication
using Zigbee and LoRaWAN - Multi-node system architecture

**Technologies:** C · MSP430 · STM32 · Raspberry Pi · Embedded Linux ·
Zigbee · LoRaWAN

> **What it demonstrates:** End-to-end IoT integration from
> microcontroller sensor nodes to a Linux-based gateway.

------------------------------------------------------------------------

### 4. Intelligent Insecticide Sprayer --- BEng Thesis

A vision-assisted insecticide spraying system implemented on an unmanned
ground vehicle (UGV).

**Highlights** - Real-time plant classification - Viola--Jones detection
and image segmentation - Raspberry Pi with Embedded Linux -
Multithreaded implementation - Processing of active image regions to
reduce computation on constrained hardware

**Technologies:** Embedded Linux · Raspberry Pi · Computer Vision ·
Image Processing · Multithreading

> **What it demonstrates:** Embedded vision, real-time processing and
> practical optimization for resource-constrained hardware.

------------------------------------------------------------------------

### 5. Event-Camera Optical Flow --- MSc Thesis

Research project investigating optical flow estimation from event-camera
data.

**Highlights** - Compared Contrast Maximization and neural-network-based
approaches - Evaluated methods using Python, PyTorch and OpenCV -
Focused on event-based vision and optimization methods

**Technologies:** Python · PyTorch · OpenCV · Computer Vision · Event
Cameras

> **What it demonstrates:** Applied research, computer vision,
> optimization and machine-learning evaluation.

------------------------------------------------------------------------

### 6. Line-Following Robot

A mobile robotics project implementing closed-loop motor control.

**Highlights** - PID-based motor control - PWM motor actuation -
Infrared sensor feedback

**Technologies:** Embedded C · PID Control · PWM · IR Sensors

> **What it demonstrates:** Control systems, timers, PWM and
> sensor-feedback integration.

------------------------------------------------------------------------

## 💼 Professional Experience

**Embedded Software Engineer --- TU Chemnitz** - Developed ESP32
firmware for a LoRaWAN communication system. - Implemented multithreaded
firmware and synchronization mechanisms. - Worked with payload
fragmentation and EU868 radio constraints. - Validated firmware on
physical hardware through extended testing. - Developed Python tooling
for server-side communication and MQTT forwarding.

**Service Engineer --- Analytical Measuring Systems** - Installed,
commissioned and maintained analytical measuring systems at customer
sites. - Performed on-site hardware and software troubleshooting.

**Independent Embedded Development** - Building C-based portfolio
projects, including a modular communication framework. - Further
developing skills in FreeRTOS and Zephyr. - Using AI-assisted
development tools to support code review, debugging and unit testing.

------------------------------------------------------------------------

## 🎯 Current Focus & Learning

I am continuing to deepen my embedded systems knowledge, with particular
interest in topics relevant to production-grade firmware and embedded
product development.

-   FreeRTOS and Zephyr RTOS
-   Yocto Project and Embedded Linux build systems
-   U-Boot, device trees and systemd
-   CAN / CANopen and Modbus
-   BLE and low-power embedded design
-   Linux kernel and device-driver fundamentals
-   C++ for embedded applications
-   Embedded cybersecurity and the Cyber Resilience Act (CRA)

------------------------------------------------------------------------

## 🎓 Education

**MSc Embedded Systems** --- TU Chemnitz, Germany\
2021--2025

Focus areas: Real-Time Systems, Multi-Sensor Systems, Digital Components
and Architectures, Computer Vision and Digital Signal Processing.

**BEng Mechatronics** --- NUST, Islamabad\
2015--2019

Focus areas included control engineering, embedded systems and PID
control.

------------------------------------------------------------------------

## 🌍 Languages

-   English --- C1
-   German --- B2
-   Urdu / Hindi --- Native

------------------------------------------------------------------------

## 📫 Let's Connect

I'm interested in embedded software and firmware engineering
opportunities involving microcontrollers, RTOS, IoT connectivity,
Embedded Linux and hardware-oriented development.

-   **Email:** <c.razanaqvi@gmail.com>
-   **GitHub:** [github.com](https://github.com/)

------------------------------------------------------------------------

::: {align="center"}
### Building reliable systems, one layer closer to the hardware. ⚙️
:::
