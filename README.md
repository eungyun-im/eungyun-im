<h1 align="center">Eungyun Im</h1>

<p align="center">
  <b>Automotive software quality · verification · field testing</b><br>
  Autonomous driving software that holds up outside the lab.
</p>

<p align="center">
  <a href="mailto:dladmsrbs12350@kookmin.ac.kr"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white"></a>
  <a href="https://github.com/KUUVe-KMU"><img src="https://img.shields.io/badge/KUUVe--KMU-181717?style=flat-square&logo=github&logoColor=white"></a>
  <a href="https://www.kookmin.ac.kr"><img src="https://img.shields.io/badge/Kookmin_University-00356B?style=flat-square&logoColor=white"></a>
</p>

3rd-year Automotive Engineering student at Kookmin University, President of [KUUVe](https://github.com/KUUVe-KMU), the autonomous driving research club. I build perception and control for scale cars, and I care about the gap between benchmark numbers and field behavior. Tracing failures on a real car led me to software verification: designing tests from requirements, injecting faults on purpose, and measuring whether the tests themselves are any good.

---

## Featured work

One emergency-braking function, verified at four levels.

| Project | Level | What it shows |
|---|---|---|
| **[automotive-sw-qa](https://github.com/eungyun-im/automotive-sw-qa)** | Unit | Simulink model, C code and Python reference compared back to back; coverage up to MC/DC, mutation testing, requirement traceability, formal proof of the requirements and fault injection in MATLAB. |
| **[ecu-quality-gate](https://github.com/eungyun-im/ecu-quality-gate)** | ECU and network | Release gate: UDS over ISO-TP, CAN timing and security checks on a virtual bench; seven planted defects prove the suites catch them. |
| **[ecu-fault-injection](https://github.com/eungyun-im/ecu-fault-injection)** | Hardware | Lost and corrupted commands, a stuck CPU, bus-off and interrupted firmware updates on an STM32. One suite for simulation and board; the board run is pending. |
| **[llm-testcase-review](https://github.com/eungyun-im/llm-testcase-review)** | Test design | LLM-written test cases measured by executing them on reference and defect versions, then repaired with feedback. |

```mermaid
flowchart LR
    A[automotive-sw-qa<br>function and test design] -- on an ECU --> B[ecu-quality-gate<br>diagnostics, network, release]
    A -- reference and baseline --> C[llm-testcase-review<br>LLM-written tests]
    B -- virtual ECU to real MCU --> D[ecu-fault-injection<br>safety mechanisms on STM32]
```

---

## Stack

![ROS2](https://img.shields.io/badge/ROS2_Jazzy-22314E?style=flat-square&logo=ros&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB_%2F_Simulink-0076A8?style=flat-square&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![CAN](https://img.shields.io/badge/CAN_%2F_UDS-555555?style=flat-square&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)

---

## Experience and awards

`2026.01 — now` President, KUUVe (Kookmin University Unmanned Vehicle)  
`2025.06 — now` Field Test Engineer, KUUVe Scale Car Project  
`2023 — now` &nbsp;&nbsp;B.E. Automotive Engineering, Kookmin University

| Date | Competition | Award |
|---|---|---|
| 2026.10 | Autonomous Robot Race, Round 3 | **Excellence Award (3rd)** |
| 2026.07 | SEA:ME Hackathon (Volkswagen Foundation) | **Gold Prize** |
| 2026.03 | 5th Int'l University EV Autonomous Driving Competition | **Effort Award** |
| 2025.11 | International Robot Contest, TurtleBot3 Autorace | **Encouragement Award** |
