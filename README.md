<h1 align="center">Danial Parviz</h1>

<p align="center">
  <b>Computer Engineering @ UT Dallas</b> · Class of May 2027 · NASA L'SPACE Alumnus<br>
  Embedded systems · FPGA acceleration · Avionics · Hardware-software integration
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/danial-parviz-5075a2212/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:dxp210034@utdallas.edu"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/Seeking-Summer%202027%20Internships%20%26%20Full--Time-2ea44f?style=flat-square" alt="Seeking">
</p>

---

## 👋 About

Senior Computer Engineering student who works where hardware meets software: FPGA accelerator
runtimes, flight avionics, rover electronics, and embedded AI. I'm looking for **Summer 2027
internships and full-time roles** in embedded systems, FPGA engineering, avionics, and
aerospace/defense.

## 🔭 Currently working on

| | Project | Where |
|---|---|---|
| 🔧 | Python runtime for a Zynq UltraScale+ FPGA accelerator *(private lab repo)* | EACAS Lab, UTD |
| 🚀 | Level 3 rocket flight computer and GPS/LoRa telemetry | AIAA Comet Rocketry |
| 🕶️ | Offline AI smart-glasses navigation system for the visually impaired | Senior Design (Blind Assistance Navigator) |
| 🔒 | Open-source MCP server security scanner | GDSC sprint team |
| 🌐 | End-to-end IoT / edge AI capstone | UTD IoT Laboratory |

---

## 🔬 Research

### EACAS Lab, UT Dallas · Undergraduate Research Assistant
*Efficient AI Computing and Accelerator Systems, under Dr. Mohamed Ibrahim*

- Lead the **ARM-side Python runtime** and a **software mock backend** (register file, kernel-load state machine, DMA loopback, failure injection) for a Zynq UltraScale+ ZCU102 FPGA accelerator used in a real-time turbulence digital twin: AXI4-Lite register access, DMA (MM2S/S2MM) data movement, kernel table loading, and failure-injection testing decoupled from physical hardware
- **8 pull requests, 2,500+ lines** of production Python; test suite grown from **0 to 30** unit and integration tests; numerical validation against **DOLFIN (FEniCS)** and **Incompact3d** at **2×10⁻⁵ relative L2 tolerance**
- Transitioning with the lab's **Fall 2026 pivot** to an event-triggered turbulence digital twin direction — co-authoring **RAPHAT**, a research manuscript targeting DAC on a reconfigurable FPGA architecture that derives its kernels directly from the governing PDE and reconfigures on-device as the physical system changes state
- Conducted a literature review of FPGA-accelerated PDE solvers (spectral/FFT methods, lattice Boltzmann, algebraic multigrid, dynamic partial reconfiguration) and synthesized a state-transition-to-hardware-mechanism mapping informing the paper's reconfigurable datapath and hardware co-design

*Code lives in a private lab repository; the team is working toward publication.*

---

## 🚀 Aerospace & NASA

### AIAA Comet Rocketry · UT Dallas

**Flight Computer & GPS Systems Engineer** · Sep 2024 – Present
- Led end-to-end avionics for a high-powered **L1 certification rocket**: full ESP32 subsystem from schematic to flight validation, multi-rail PCB power distribution, SMT assembly, and hardware bring-up — deterministic bare-metal C++ firmware achieving **50 Hz acquisition, <2 ms jitter**, BMP280 altimeter over I2C, SPI microSD logging of 20+ flight parameters through apogee and recovery
- Advanced to the team's current **L3 program**, researching and proposing an upgraded flight computer around the **STM32H743 (Cortex-M7)**: hardware FPU for Kalman-filter sensor fusion, integrated FDCAN, and dedicated SPI buses to move sensors off a shared I2C bus
- Sensor suite selection, **IREC 2026 DTEG** compliance analysis, CAN bus architecture (CANaerospace), and FreeRTOS firmware planning
- GPS telemetry and long-range **LoRa** ground-station communication for real-time tracking and recovery, across both rocket programs

**Flight Simulation Engineer** · Mar 2026 – Sep 2026
- **6-DOF trajectory simulation** (RocketPy) predicting apogee within **2%** for a 10,000 ft Spaceport America Cup rocket
- **Monte Carlo dispersion analysis** across 1,000+ iterations
- Backwards-physics engine for optimal **airbrake deployment**; ANSYS Fluent CFD drag data turned into lookup tables for the flight computer
- Python multiprocessing framework that cut design iteration time by **75%**

### NASA Lunabotics Challenge · Electrical Systems Engineer
- Architected the rover's **triple 3S LiPo power distribution** and voltage regulation for drivebase, compute, and sensors
- Designed the electrical enclosure for a Jetson Nano and ESP32 control electronics, from schematic through 3D model to physical build
- Built the **CAN bus** link from the ESP32 to dual SPARK MAX motor controllers; traded a custom transceiver PCB for a manufactured chip to protect the supply chain against tariff constraints
- Diagnosed and corrected a reversed-polarity wiring fault; led integration and power budgeting; co-authored the NASA **Systems Engineering Paper** and Robot Data Report

### NASA L'SPACE Mission Concept Academy · CDH Systems Engineer
*Lunar south pole rover mission (Aquarius)*
- Designed the full command and data handling architecture through four gate reviews (MCR, SRR, MDR, PDR)
- Trade study of **RAD750, LEON4FT, and SpaceCube Mini**; selected the RAD750 for radiation hardness and flight heritage
- Traceable requirements (64 GB storage, 256 kbps X-band downlink, redundant fault recovery); X-band telecom with a **MIL-STD-1553** dual-redundant bus

---

## 🧠 Embedded AI & Software

**Senior Design · Embedded AI & Systems Engineer — Blind Assistance Navigator**
Offline-first AI smart-glasses navigation system for individuals with visual impairments. Designing a modular wearable (NVIDIA Jetson Orin Nano, FPGA acceleration, stereo-depth cameras, custom STM32 hardware) with a real-time perception pipeline (PyTorch, CUDA, TensorRT) fusing object detection, depth estimation, ToF proximity sensing, IMU, and GPS. Exploring quantized vision-language models for offline scene understanding, and planning FPGA-based depth-map filtering (Vitis HLS/RTL) benchmarked against a CPU baseline. 6-person interdisciplinary team.

**IoT & Edge AI Systems** · UTD IoT Laboratory
- MQTT sensor-to-cloud pipelines on Raspberry Pi with dashboards and actuator control
- **TinyML** deployment benchmarked against cloud inference (accuracy, latency, memory)
- Small Language Model **agentic workflows** with tool calling for device management
- **AWS IoT Core** telemetry ingestion, event-driven alerts, and ML inference
- 15-week capstone prototype with a live demo and technical poster

**MCP Security Scanner** · GDSC sprint team
Open-source CLI scanner for Model Context Protocol servers: over-privileged tool permission detection, severity scoring, **SARIF output** for GitHub Code Scanning, and a labeled benchmark corpus of intentionally vulnerable servers.

**Critique AI** · Backend engineer
AI writing-feedback tool that helps students improve without rewriting for them. Built the Gemini integration, the `/api/analyze` endpoint (retries, validation), and the `/api/extract` PDF/Word extraction endpoint.

---

## ⚡ Digital & Power Design

**48-bit Harvard RISC Processor** · [repo](https://github.com/DanialParviz/48-bit-harvard-risc-processor)
Custom 48-bit ISA with a multi-cycle Harvard architecture, 13-bit address bus (8,192 locations), ALU, register file, program counter, and FSM control logic. Verified through RTL simulation and waveform analysis in ModelSim/Vivado.

**Wind Energy Power Electronics** · UTD Wind Energy Club
Three-phase AC-DC rectifier for a wind generator load side: LC filter modeling in LTSpice, MOSFET high-current load switching, and Altium PCB layout, validated with oscilloscope measurements.

---

## 🛠️ Tech Stack

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Verilog](https://img.shields.io/badge/Verilog%20%2F%20SystemVerilog-8A2BE2?style=flat-square)
![VHDL](https://img.shields.io/badge/VHDL-5C6BC0?style=flat-square)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**FPGA & Digital**
![Vivado](https://img.shields.io/badge/Vivado-E4002B?style=flat-square)
![Vitis HLS](https://img.shields.io/badge/Vitis%20HLS-E4002B?style=flat-square)
![ModelSim](https://img.shields.io/badge/ModelSim-1F6FEB?style=flat-square)
![Zynq](https://img.shields.io/badge/Zynq%20UltraScale%2B-ED1C24?style=flat-square)
![PYNQ](https://img.shields.io/badge/PYNQ-F7931E?style=flat-square)
![AXI4-Lite](https://img.shields.io/badge/AXI4--Lite%20%2F%20DMA-555?style=flat-square)

**AI & Edge Inference**
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)
![TensorRT](https://img.shields.io/badge/TensorRT-76B900?style=flat-square&logo=nvidia&logoColor=white)
![VLMs](https://img.shields.io/badge/Vision--Language%20Models-555?style=flat-square)

**Embedded**
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)
![STM32H743](https://img.shields.io/badge/STM32H743-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![Jetson](https://img.shields.io/badge/Jetson%20Orin%20Nano%20%2F%20Nano-76B900?style=flat-square&logo=nvidia&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![Embedded Linux](https://img.shields.io/badge/Embedded%20Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![PlatformIO](https://img.shields.io/badge/PlatformIO-F5822A?style=flat-square&logo=platformio&logoColor=white)
![FreeRTOS](https://img.shields.io/badge/FreeRTOS-6DB33F?style=flat-square)

**Protocols:** `SPI` · `I2C` · `UART` · `CAN` · `FDCAN` · `LoRa` · `MQTT` · `MIL-STD-1553`

**PCB & Analysis**
![Altium](https://img.shields.io/badge/Altium-F5A800?style=flat-square)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=flat-square&logo=kicad&logoColor=white)
![LTSpice](https://img.shields.io/badge/LTSpice-444?style=flat-square)
![ANSYS Fluent](https://img.shields.io/badge/ANSYS%20Fluent-FFB71B?style=flat-square)
![RocketPy](https://img.shields.io/badge/RocketPy-D33?style=flat-square)

**Software & Cloud**
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS IoT](https://img.shields.io/badge/AWS%20IoT%20Core-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

---

## 🏆 Recognition & More

- President's Education Award · Certificate of Congressional Recognition
- Languages: English, Persian (native/bilingual)
- Co-founder, **UTD Backgammon Club**: campus tournaments and community events
- Division II collegiate rugby athlete
- Member, IEEE

---

<p align="center">
  <i>Open to opportunities in embedded systems, FPGA engineering, avionics, and aerospace/defense.</i><br>
  <a href="https://www.linkedin.com/in/danial-parviz-5075a2212/">LinkedIn</a> ·
  <a href="mailto:dxp210034@utdallas.edu">dxp210034@utdallas.edu</a>
</p>
