<div align="center">
<img src="https://komarev.com/ghpvc/?username=CyrusRaza" width="1" height="1" alt="" />

# Hi, I'm Cyrus Naqvi 👋

### Embedded Software Engineer | Firmware | IoT Connectivity | Edge Vision

I build firmware that holds up on real hardware: concurrent C on microcontrollers, wireless links that don't drop data, and test pipelines that catch problems before hardware does.

[![Email](https://img.shields.io/badge/Email-c.razanaqvi%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:c.razanaqvi@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/cyrus-naqvi-b96282194/)

📍 Berlin, Germany · MSc Embedded Systems, TU Chemnitz · Open to embedded and firmware roles across Germany

</div>

---

## What I bring

- **Firmware ownership.** Sole developer of the ESP32 firmware for a LoRaWAN communication system at TU Chemnitz: architecture, concurrency, radio protocol handling and hardware validation.
- **Reliability you can measure.** Resend-on-missing-ACK logic that delivered **0 lost packets in a 24-hour continuous run** on real hardware.
- **Real-time concurrency.** FreeRTOS tasks, mutexes and semaphores in real device firmware; lock-free ring buffers and C11 threads in my own frameworks.
- **Clean, testable C.** Strategy pattern with function-pointer tables, opaque objects, Unity unit tests, CMake and GitHub Actions CI on every push.
- **Hardware in the field.** Installation, calibration and repair of analytical instruments (electron microscopes, UV spectroscopes) at customer sites: part of about 10 installations and 50+ calibrations.

---

## Featured Projects

### 🔌 [IoT Device Simulator: Modular Transport and Command Framework in C](https://github.com/CyrusRaza/iot_device_sim)
A simulated IoT edge device that receives commands over a runtime-selectable transport and applies them to device state.

- MQTT client (libmosquitto) and WebSocket server (libwebsockets) behind one function-pointer interface: new transports plug in without touching application code
- Producer/consumer split: transport callbacks feed a bounded ring buffer with C11 atomics and semaphores; a dedicated parser thread applies commands under a mutex
- **43 Unity tests**, CMake, Docker Compose broker, GitHub Actions CI

**Stack:** C11 · MQTT · WebSocket · C11 threads · Unity · CMake · Docker · GitHub Actions

### 👁️ [Motion-Gated ROI Extraction for Edge AI on Microcontrollers](https://github.com/CyrusRaza/stm32-sparse-vision)
Event-camera-inspired sparse processing on a conventional camera: detect what moved, cut the frame down to a few regions of interest, and run the detector only there. Target: STM32H7 (Cortex-M7, 480 MHz).

- Luma-only frame differencing, thresholding and morphology, then two ROI strategies: contours and a recursive X-Y cut that needs **under 2 KB of memory**
- Evaluation harness against the **CDnet 2014** benchmark with pixel-level recall/precision and per-stage timing
- Separate PC and Cortex-M7 CMake targets with cross-compilation, both built in CI

**Stack:** C++20 · OpenCV · STM32H7 · arm-none-eabi-gcc · CMake · GitHub Actions

### 🎯 [motpipe: Multi-Object Tracking Pipeline](https://github.com/CyrusRaza/motpipe)
Detection and tracking framework with detectors and trackers swappable at runtime.

- YOLOv8, YOLOv5, Faster R-CNN and SSD detectors; SORT, DeepSORT and ByteTrack trackers, all behind two interfaces and a registry
- Installable Python package with a CLI, optional extras and CI
- Benchmarked every pair: **56 FPS at 1080p** with YOLOv8n + ByteTrack on an RTX 3050 laptop GPU, tracking under 2 ms per frame

**Stack:** Python · PyTorch · OpenCV · YOLO · ByteTrack · GitHub Actions

---

## Experience

**Embedded Software Engineer | TU Chemnitz** (Oct 2023 - Oct 2025)
- Designed and built the complete C firmware for a LoRaWAN communication system on ESP32 as the sole embedded developer
- Structured the firmware into concurrent FreeRTOS tasks for main logic, sending and receiving, synchronised with mutexes and semaphores
- Implemented payload fragmentation within EU868 duty-cycle limits and drove the LoRaWAN module over UART with AT commands
- Built a LoRaWAN alternative to the Wi-Fi data path of an external company's IOTA platform, using its encryption API
- Wrote the Python tooling that forwarded device data over MQTT, and integrated the device with the server team's software
- Validated on real hardware: 0 packets lost in a 24-hour continuous run

**Student Research Assistant | TU Chemnitz** (Sep 2023 - Mar 2024)
- Developed MATLAB/Simulink software drivers for PID control experiments in control engineering teaching

**Service Engineer | Analytical Measuring Systems, Karachi** (Dec 2019 - Apr 2021)
- Installed, commissioned, calibrated and repaired electron microscopes and UV spectroscopes at customer sites
- Diagnosed hardware and software faults on site and documented the service work

---

## More Projects

- **IoT Smart Irrigation:** multi-node system with MSP430 sensor nodes, an STM32L4 gateway (my firmware, STM32CubeIDE + HAL) and a Raspberry Pi running Embedded Linux, over Zigbee and LoRaWAN
- **CWE Weakness Handling (MSc research project):** extended a Django requirements engineering tool with MITRE CWE import, schema validation, search and project linking, with a full test campaign
- **Event-Camera Optical Flow (MSc thesis):** compared contrast maximization with neural-network approaches in Python and PyTorch
- **Intelligent Insecticide Sprayer (BEng thesis):** real-time, multithreaded plant classification on a Raspberry Pi mounted on a UGV
- **Line-Following Robot:** closed-loop PID motor control with PWM and IR feedback

---

## Tech Stack

| | |
|---|---|
| **Languages** | C, Python, C++, MATLAB |
| **Microcontrollers** | ESP32, STM32 (ARM Cortex-M), MSP430, Raspberry Pi |
| **RTOS & OS** | FreeRTOS, bare-metal, Embedded Linux |
| **Connectivity** | LoRaWAN (EU868), Zigbee, MQTT, WebSocket |
| **Interfaces** | UART, SPI, I²C, PWM, ADC, GPIO, timers |
| **Concurrency** | tasks and threads, mutexes, semaphores, lock-free ring buffers |
| **Build, Test & CI** | CMake, Git, Unity, GitHub Actions, Docker |
| **Vision & ML** | OpenCV, PyTorch, TensorFlow, NumPy, event cameras |
| **Also worked with** | Zephyr, GDB, JTAG/SWD, oscilloscope, logic analyzer, VHDL, Django, SQLite |

<div align="center">

![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FreeRTOS](https://img.shields.io/badge/FreeRTOS-2C3E50?style=flat-square)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-C51A4A?style=flat-square&logo=raspberrypi&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=flat-square&logo=cmake&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

</div>

---

## Education

**MSc Embedded Systems** | TU Chemnitz, Germany (2021 - 2025)
Real-Time Systems, Multi-Sensor Systems, Digital Architectures, Computer Vision, Digital Signal Processing

**BEng Mechatronics** | NUST, Islamabad (2015 - 2019)
Control Engineering, Embedded Systems, PID Control

## Languages

English (C1) · German (B2) · Urdu / Hindi (Native)

---

<div align="center">

**Looking for my next embedded or firmware role in Germany. Let's talk.**

[Email](mailto:c.razanaqvi@gmail.com) · [LinkedIn](https://www.linkedin.com/in/cyrus-naqvi-b96282194/)

</div>
