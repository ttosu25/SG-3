# Strain Gauge Measurement System (Load Sensing Node)

## 1. Project Overview

You are required to design and implement a low-cost strain measurement system for monitoring mechanical strain on a loaded beam. The system will acquire strain data from a resistive strain gauge, condition the signal, and provide a digital output for logging and analysis.

The design should be suitable for laboratory testing and demonstrate correct analog signal conditioning principles.

## 2. Functional Requirements

The system shall:

Measure strain using a bonded resistive strain gauge
Convert strain into a usable electrical signal via a Wheatstone bridge
Condition the signal using analogue circuitry
Output a digital representation of strain for logging or display
Operate continuously under static or slowly varying loads

## 3. Sensor Requirements
Strain gauge nominal resistance: 350 Ω
Gauge factor: 2.0 ± 5%
Mounting: quarter-bridge configuration (unless justified otherwise in design)
Maximum strain range: 0 to 1200 µε
Assume linear elastic behaviour of the test specimen

## 4. Electrical Requirements

Excitation
Bridge excitation voltage: 3.3 V or 5 V (designer choice)
Excitation must be stable within ±1%
Signal Conditioning
Instrumentation amplifier required
Output must be scaled to ADC input range
Gain must be adjustable or justified analytically
Noise / Accuracy Targets
Minimum resolution target: ≤ 5 µε
Total system non-linearity: < 1% full scale
Drift over 10 minutes: must be minimised and characterised

## 5. Data Conversion
Microcontroller-based ADC required
ADC resolution: ≥ 12-bit
Sampling rate: ≥ 50 Hz
Output format: serial (UART / USB / equivalent)

## 6. Mechanical Assumptions
Strain gauge is correctly bonded to a uniform metallic beam
Beam behaves within elastic region (Hooke’s law valid)
Temperature is approximately constant (20–25°C), but drift effects should be discussed

## 7. Environmental Constraints
Laboratory environment (non-industrial)
No significant vibration or EMI shielding provided
Cable lengths: up to 1 m between sensor and conditioning circuit

## 8. Design Constraints
System must be constructed using readily available components (no custom IC fabrication)
PCB design encouraged but not mandatory
Power supply limited to 5 V USB or bench supply
Total system cost target: < £50 in components

## 9. Deliverables

You must submit:

Full circuit schematic (hand-drawn or CAD)
Design calculations (bridge output, gain, resolution analysis)
Simulation results (bridge + amplifier stage)
Working prototype or demonstrator
Calibration method and results
Technical report (max 15 pages)