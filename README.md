[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=13&duration=3000&pause=1000&color=58A6FF&width=500&lines=AUTOMOTIVE+SW+QUALITY+%C2%B7+VERIFICATION+%C2%B7+FIELD+TESTING)](https://github.com/eungyun-im)

# Eungyun Im

Building autonomous driving software that holds up outside the lab.

I'm a 3rd-year Automotive Engineering student at Kookmin University. I develop perception and control systems for scale cars through [KUUVe](https://github.com/KUUVe-KMU), the autonomous driving research club I lead. I care about the gap between benchmark numbers and real-world field behavior, and about building the process that closes it.

Tracing failures on a real car is what led me to software verification: designing tests from requirements, injecting faults on purpose, and measuring whether the tests themselves are any good.

[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:dladmsrbs12350@kookmin.ac.kr)
[![KUUVe](https://img.shields.io/badge/KUUVe--KMU-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/KUUVe-KMU)

---

## Focus areas

**Autonomous driving stack** — Integrating perception, localization, and control end-to-end on a real vehicle and validating behavior through repeated field tests.

**Edge AI deployment** — Getting inference models onto constrained hardware and verifying that speed and accuracy hold across devices and conditions.

**Field fault isolation** — Tracing failures from symptom to root cause through logs, layer by layer, until the fix is provable and the regression is documented.

---

## Featured work

Three projects verify the same automatic emergency braking function at three levels: the unit, the ECU on its network, and the test design process itself. A fourth takes the question to real hardware: do the safety mechanisms of an ECU work when the fault actually happens?

| Project | Level | What it does |
|---|---|---|
| **[automotive-sw-qa](https://github.com/eungyun-im/automotive-sw-qa)** | Software unit | Requirement-based testing of one function in three forms (Simulink/Stateflow model, C code, Python reference) compared back to back, with the test design measured by coverage up to MC/DC and by mutation testing. |
| **[ecu-quality-gate](https://github.com/eungyun-im/ecu-quality-gate)** | ECU and network | Release gate for ECU software. UDS diagnostics over ISO-TP (udsoncan, can-isotp, python-can), CAN timing and security checks run on a virtual bench, and a build with seven planted defects proves the suites catch them. |
| **[ecu-fault-injection](https://github.com/eungyun-im/ecu-fault-injection)** | ECU on hardware | Fault injection bench for an STM32 ECU. Lost and corrupted commands, a stuck CPU, bus-off and interrupted firmware updates over CAN are injected on purpose. One test suite is written for both simulation and the board: it passes in simulation, and the run on the board is pending. |
| **[llm-testcase-review](https://github.com/eungyun-im/llm-testcase-review)** | Test design research | Measures LLM-written test cases by executing them on reference and defect versions, and repairs the test set with boundary, cross-check and mutation feedback. |

```mermaid
flowchart LR
    A[automotive-sw-qa<br>AEB decision logic<br>and its test design] -- same function, on an ECU --> B[ecu-quality-gate<br>diagnostics, network,<br>security, release verdict]
    A -- reference implementation<br>and human baseline --> C[llm-testcase-review<br>how good are<br>LLM-written tests?]
    B -- from a virtual ECU<br>to a real MCU --> D[ecu-fault-injection<br>safety mechanisms and<br>firmware update on an STM32]
```

---

## Stack

**Autonomous driving**

![ROS2](https://img.shields.io/badge/ROS2_Jazzy-22314E?style=flat-square&logo=ros&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)

**Software quality and verification**

![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![CAN](https://img.shields.io/badge/CAN_%2F_UDS-555555?style=flat-square&logoColor=white)
![ISO-TP](https://img.shields.io/badge/ISO--TP-555555?style=flat-square&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)


---

## Experience

`2026.01 — Present` &nbsp; President — KUUVe · Kookmin University Unmanned Vehicle  
`2025.06 — Present` &nbsp; Field Test Engineer — KUUVe Scale Car Project  
`2023 — Present` &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; B.E. Automotive Engineering — Kookmin University

---

## Awards

| Date | Competition | Award |
|---|---|---|
| 2026.07 | SEA:ME Hackathon (Volkswagen Foundation) | **Gold Prize** |
| 2026.10 | Autonomous Robot Race, Round 3 | **Excellence Award (3rd)** |
| 2026.03 | 5th Int'l University EV Autonomous Driving Competition | **Effort Award** |
| 2025.11 | International Robot Contest — TurtleBot3 Autorace | **Encouragement Award** |
