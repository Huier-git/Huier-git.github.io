---
layout: page
permalink: /project/index.html
title: Projects
---

# Research Projects

<br>

#### [Multi-Rod Planetary Regolith Drilling Robot](#)

<center>
<img src="/images/projects/multi-rod-prototype.png" alt="Multi-rod drilling robot prototype — four-stage operation sequence">
</center>
<p class="img-caption">Silhouette of the multi-rod cyclic operation sequence on the prototype</p>

A deep-regolith sampling system for lunar exploration. Independently completed full-stack R&D across control system design, motion planning, soil-tool interaction modeling, and deep learning.

- **Role** &mdash; Project Lead &middot; Master's Thesis &middot; NSFC Project
- **Lab** &mdash; GDUT Biomimetic & Intelligent Robotics Lab
- **Timeline** &mdash; 2023.06 &ndash; Present

**Key contributions**

1. **Control System** &mdash; Built a 9-DOF drilling robot platform with EtherCAT + Modbus dual-bus architecture; HMI features 5-thread parallelism, 7-state FSM, and safety interlocks.
2. **Motion Planning** &mdash; Modeled multi-rod cooperative sequencing as an RCPSP problem; solved via Petri net + MILP + CP-SAT for globally optimal rod scheduling (&ge;4.9% improvement).
3. **Mechanics Modeling** &mdash; Proposed a multi-component coupled soil-tool interaction model (Janssen + Terzaghi + PFRT + Coulomb); experimentally validated with &plusmn;18% prediction error.
4. **Deep Learning** &mdash; Built a physics-guided classification model with physical-prior force-ratio features; achieved cross-domain transfer F1&nbsp;=&nbsp;0.736 (+16.7 pp over baseline).

<div class="img-row">
<img src="/images/projects/multi-rod-architecture.png" alt="EtherCAT + Modbus dual-bus control architecture">
<img src="/images/projects/multi-rod-prfinet.png" alt="PRFINet — physics-guided deep learning architecture">
</div>
<p class="img-caption">Left: Dual-bus control system architecture &nbsp;&middot;&nbsp; Right: PRFINet deep learning model</p>

**Tech stack** &mdash; `EtherCAT` `Modbus` `Qt / C++` `PyTorch` `OR-Tools` `Petri Net` `SQLite` `Optuna`

**Output** &mdash; 1 prototype, 2 invention patents (1 granted), 1 software copyright, 1 EI conference paper, 2 SCI journal papers.

<br>

---

#### [Vacuum-Cryogenic Drill Temperature Monitoring System](#)

<center>
<img src="/images/projects/vacuum-cryogenic-drill.png" alt="Instrumented ice-drill prototype">
</center>
<p class="img-caption">Instrumented ice-drill prototype with thermocouple wiring</p>

<div class="img-row">
<img src="/images/projects/thermocouple-install.png" alt="Thermocouple embedding on spiral drill bit">
<img src="/images/projects/temp-scanner-board.png" alt="Multi-channel temperature scanner PCB">
</div>
<p class="img-caption">Left: Thermocouple embedding on spiral drill bit &nbsp;&middot;&nbsp; Right: Multi-channel temperature scanner board</p>

Commissioned by Beijing Institute of Satellite Manufacturing (Factory 529). Delivered a full temperature monitoring solution for lunar water-ice drilling at &minus;190&nbsp;&deg;C under vacuum &mdash; covering system design, hardware/software development, and mechanical integration.

- **Role** &mdash; System Architect & Project Lead
- **Client** &mdash; Beijing Institute of Satellite Manufacturing (Factory 529)
- **Timeline** &mdash; 2025.07 &ndash; Present

**Key contributions**

1. **System Design** &mdash; Designed a 10-channel micro-thermocouple embedding scheme with slip-ring routing and anti-wear protection for reliable signal acquisition under extreme conditions.
2. **Hardware** &mdash; Designed a multi-channel temperature scanner based on STM32G030 + ZAM6218, with Modbus / RS-485 uplink.
3. **Software** &mdash; Developed a cross-platform acquisition application supporting 100&nbsp;Hz sampling, 5M+ data points, multi-point calibration, and CSV import/export.
4. **Thermal Analysis** &mdash; Built a thermal-resistance / thermal-capacitance equivalent model; performed coupled thermal-structural verification with SolidWorks Simulation.

**Tech stack** &mdash; `STM32` `ZAM6218` `Modbus RTU` `RS-485` `Tauri` `Web Serial API` `Thermal Modeling`

**Output** &mdash; 1 instrumented ice-drill prototype, 1 monitoring system, 1 software copyright, 1 invention patent.

<br>

---

#### [Compact EtherCAT Servo Drive](#)

<div class="img-row">
<img src="/images/projects/motor-driver.png" alt="Compact EtherCAT servo drive PCB">
<img src="/images/projects/motor-driver-assembled.png" alt="Assembled servo drive with EtherCAT module">
</div>
<p class="img-caption">Left: PCB layout with three-phase inverter &nbsp;&middot;&nbsp; Right: Assembled unit with EtherCAT module</p>

A compact, high-performance servo drive for brushless motors, designed to serve as the actuator controller in the multi-rod drilling robot system. Implements field-oriented control (FOC) with EtherCAT real-time communication for multi-axis coordination.

- **Role** &mdash; Hardware & Firmware Developer
- **Timeline** &mdash; 2024.09 &ndash; Present
- **Platform** &mdash; STM32, three-phase MOSFET inverter, magnetic encoder (SPI), EtherCAT slave module

**Key contributions**

1. **Hardware** &mdash; Designed a compact 4-layer PCB integrating three-phase inverter, current sampling, magnetic encoder interface, EtherCAT communication module, and OLED display.
2. **FOC Algorithm** &mdash; Implemented field-oriented control with Park/Clarke transforms, PI current loop at 20 kHz PWM, supporting torque / velocity / position cascade control modes.
3. **EtherCAT Integration** &mdash; Achieved deterministic real-time communication via SPI-based EtherCAT slave, enabling synchronized multi-axis motion in the drilling robot.
4. **Calibration & Diagnostics** &mdash; Built motor parameter auto-identification, encoder calibration routines, and a command-line shell for real-time debugging.

**Tech stack** &mdash; `STM32` `FOC` `EtherCAT` `FreeRTOS` `SPI` `CAN` `PCB Design`

**Output** &mdash; 1 functional drive board, integrated into the drilling robot control system.

<br>

---

#### [Portable Folding Hand-Held Drill for Astronaut Use](#)

<center>
<img src="/images/projects/portable-folding-drill.png" alt="Portable folding hand-held drill prototypes">
</center>

A foldable hand-held drill stand for astronaut coring operations, featuring automatic feed, compact triple-fold frame, and extreme-environment tolerance.

- **Role** &mdash; Mechanical Designer
- **Client** &mdash; Beijing Institute of Satellite Manufacturing (Factory 529)
- **Timeline** &mdash; 2025.03 &ndash; 2025.06
- **Key work** &mdash; Rope-drive auto-feed module, triple-fold frame, motor/drive selection (Maxon + Elmo), simulation-based strength & stiffness verification
- **Output** &mdash; 1 engineering prototype, validated by ground tests

<br>

---

# Internship Experience

<br>

#### Beijing Institute of Satellite Manufacturing (Factory 529)

**Engineering Systems R&D Intern** &nbsp;&middot;&nbsp; 2025.06 &ndash; 2025.09

- Hardware & software development of temperature monitoring for drill tools under vacuum-cryogenic conditions
- Independent thermocouple integration design and vacuum chamber test setup
- Multi-channel real-time data acquisition software development
- 3D modeling, test coordination, and technical documentation

<br>

#### Guangzhou Quality Supervision & Testing Institute

**Quality Inspection Intern** &nbsp;&middot;&nbsp; 2023.08 &ndash; 2023.09

- Optical thickness measurement of insulation and sheath materials for cable products
- Tensile, crack-resistance, thermal-aging, and ductility tests per national standards
- Resistance measurement and co-authoring inspection reports
