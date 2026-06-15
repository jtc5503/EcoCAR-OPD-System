> [!IMPORTANT]
> **Proprietary Information & NDA Compliance**
> This project was completed as part of the EcoCAR EV Challenge in partnership with General Motors and the U.S. Department of Energy. Due to the proprietary nature of the vehicle platform (Cadillac LYRIQ) and competition-specific software, certain technical models, source code, and detailed CAD data are protected under a Non-Disclosure Agreement (NDA). The documentation provided here focuses on high-level system architecture, control logic methodology, and safety-critical analysis permitted for public disclosure.
# EcoCAR EV Challenge: One-Pedal Drive & Braking System
**Co-Lead Simulink Engineer | Model-Based Design | System Safety**

## Project Overview
Redesigned the One-Pedal Drive (OPD) and braking architecture for a Cadillac LYRIQ. This involved complex integration of regenerative braking and friction braking to ensure a seamless driver experience and system safety.

## Technical Contributions
* **Braking System Redesign:** Integrated friction brake blending with regenerative braking models in Simulink.
* **Control Architecture:** Developed 2D pedal maps to calibrate torque demand vs. pedal travel.
* **Safety Engineering:** Conducted a formal **Preliminary Hazard Analysis (PHA)**, ensuring automatic system disablement and driver notification during critical faults.
* **Validation:** Iteratively tuned control gains to balance energy recovery with luxury vehicle "feel".

## Tools Used
* **Modeling:** Simulink, MATLAB.
* **Hardware-in-the-Loop:** Vehicle software integration.

---

## 📊 Poster Presentations & Research

Select a presentation below to view the full academic poster and technical breakdown of the system's development lifecycle.

<details>
<summary><b>📋 2026: EcoCAR PCM Safety & Braking Validation (Senior Design)</b></summary>
<br>

### EcoCAR: PCM Safety & Braking Validation
* **Track / Focus:** Mechanical Engineering | High-Performance Vehicles Track (Senior Design 2026)
* **Team:** John Collins, Roberto Martin | **Advisor:** Dr. Patrick Currier

#### Project Overview & Key Objectives
This work presents the continued development and validation of the Propulsion Control Module (PCM) for the EcoCAR EV Challenge vehicle. Following a preliminary hazard analysis (PHA) of the complete torque path, critical safety gaps were identified in transmission interlock logic, torque limiting behavior, and braking signal coordination. 

* **Preliminary Hazard Analysis:** Evaluated the complete PCM torque path to identify safety-critical failure modes (e.g., unintended propulsion during range changes, loss of friction braking).
* **Braking Subsystem Redesign:** Integrated comprehensive fault detection (monitoring battery temp, voltage, current, SOC, and inverter states) with strict regenerative braking control and brake blending capability.
* **Transmission Interlocks:** Tightened shift parameters in Stateflow logic (Neutral ↔ Drive ↔ Reverse conditions) to completely eliminate unsafe range transitions.
* **Validation & Deployment:** Successfully validated all integrated changes via Model-in-the-Loop (MIL) simulation and compiled the complete module onto the Speedgoat real-time target machine for physical vehicle testing.
