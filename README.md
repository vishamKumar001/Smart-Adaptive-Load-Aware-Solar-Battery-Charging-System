## Smart Adaptive Load-Aware Solar Battery Charging System

## Overview

This project focuses on developing a smart solar battery charging system that combines Maximum Power Point Tracking (MPPT) with adaptive load-aware charging control.

The proposed system uses a buck-boost converter to accommodate different battery voltage configurations and dynamically adjusts its PWM duty cycle according to solar input conditions and battery requirements.

The system supports 3S and 4S battery configurations and incorporates Coulomb counting-based State of Charge (SoC) estimation for controlled charging.

## Project Objectives

- Develop an adaptive solar-powered battery charging system.
- Implement MPPT for efficient solar power extraction.
- Integrate buck-boost DC-DC conversion.
- Support multiple battery configurations (3S and 4S).
- Implement battery SoC estimation using Coulomb counting.
- Adapt charging control according to operating conditions.
- Reduce charging stress and account for inductor current ripple.

## System Architecture

Solar PV Panel → MPPT Controller → Buck-Boost Converter → Battery Pack

The controller monitors solar input and battery parameters, calculates the required PWM duty cycle, and regulates the converter operation.

## Key Features

- Adaptive MPPT control.
- Multi-objective optimization considering power extraction, battery charging current, current ripple and load mismatch.
- Right Half Plane (RHP) zero-aware adaptive step-size adjustment.
- Buck and boost operating modes.
- Coulomb counting-based SoC estimation.
- 3S and 4S battery configuration support.
- PWM-based converter control.
- Charging threshold control.

## Hardware Specifications

| Component              | Specification  |
| ---------------------- | -------------- |
| Controller             | Arduino        |
| Converter              | Buck-Boost     |
| MOSFET                 | 60 V, 30 A     |
| Inductor               | 0.5 mH         |
| Output capacitors      | 330 µF, 470 µF |
| Battery configurations | 3S and 4S      |

## Simulation and Experimental Results

The system was modelled and evaluated under different input voltage and battery configuration conditions.

### PWM Duty-Cycle Comparison

| Input | Battery | Target Voltage | Calculated Duty | Observed Duty |
| ----- | ------- | -------------- | --------------- | ------------- |
| 12 V  | 3S      | 12.6 V         | 0.512           | 0.519         |
| 12 V  | 4S      | 16.8 V         | 0.583           | 0.587         |
| 10 V  | 3S      | 12.6 V         | 0.557           | 0.558         |
| 10 V  | 4S      | 16.8 V         | 0.627           | 0.631         |
| 15 V  | 3S      | 12.6 V         | 0.456           | 0.460         |
| 15 V  | 4S      | 16.8 V         | 0.528           | 0.530         |

The simulation demonstrated adaptive PWM control and battery SoC progression. Hardware testing was also performed to observe PWM variations during charging operation.

## Tools and Technologies

- MATLAB/Simulink
- Arduino
- Power Electronics
- MPPT Control
- Buck-Boost Converter
- PWM Generation
- Battery SoC Estimation
- Embedded Control Systems

## Applications

- Solar-powered battery charging.
- Electric vehicle charging applications.
- Renewable energy storage.
- Multi-configuration battery charging.
- Battery-supercapacitor hybrid energy systems.

## Future Scope

- Battery State of Health (SoH) estimation.
- Machine learning-based battery monitoring.
- Bidirectional DC-DC converter integration.
- IoT-based remote monitoring.
- Advanced battery protection and fault detection.

## Project Contributors

Krishna Priyanka R
Vineeth S
Visham Kumar V
Seethalakshmi I
Praveen Kumar N

Department of Electrical and Electronics Engineering
Amrita Vishwa Vidyapeetham, Coimbatore, India

---

*Academic engineering project for research and educational purposes.*
