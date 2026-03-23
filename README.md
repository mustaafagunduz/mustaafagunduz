⚡ Design and SPS-Based Control of a Dual Active Bridge (DAB) DC-DC Converter

This repository presents the design, mathematical modeling, PLECS simulation, and performance analysis of a high-frequency isolated Dual Active Bridge (DAB) DC-DC converter.

The project focuses on bidirectional power transfer and closed-loop voltage regulation using Single Phase Shift (SPS) modulation.

📌 Project Overview

The proposed converter is designed for applications such as:

Energy storage systems
Electric vehicle (EV) charging
Vehicle-to-Grid (V2G) systems

It provides:

Galvanic isolation
High power density
Bidirectional energy flow capability
🔧 System Specifications
Parameter	Value
Input Voltage ($V_{in}$)	24 V
Output Voltage ($V_{out}$)	96 V
Nominal Power ($P_{nom}$)	50 W
Switching Frequency ($f_{sw}$)	100 kHz
Transformer Turns Ratio ($n$)	1:4
🛠️ Technical Features
🔹 Realistic Modeling
Includes parasitic elements and internal resistances ($0.1\ \Omega$)
Captures non-ideal effects such as losses and damping
Provides closer approximation to real hardware behavior
🔹 Control Strategy
Closed-loop PID controller
Controls the phase shift ratio ($d$) in SPS modulation
Maintains stable 96 V output under varying load conditions
🔹 Bidirectional Operation
Supports both:
Forward power transfer
Reverse power transfer (V2G mode)
Direction controlled via phase shift polarity
📊 Simulation Results (PLECS)

The system performance is validated through PLECS simulations.

✅ Steady-State Performance
Output voltage error < 0.1% at nominal load
⚡ Dynamic Response
Stable under sudden load changes:
From 200 Ω → 100 Ω
Controller compensates voltage drops caused by parasitics
🔄 V2G Mode
Bidirectional power flow successfully demonstrated
Energy transferred from secondary (110 V) back to primary side
📂 Repository Structure
/Simulation   -> PLECS model files (.plecs)
/Docs         -> Detailed technical report (Turkish)
/Figures      -> Waveforms and simulation results

📚 References

This work is based on well-established literature in isolated bidirectional converters, including:

De Doncker et al. – Dual Active Bridge concepts
B. Zhao – Control and modeling of DAB converters
