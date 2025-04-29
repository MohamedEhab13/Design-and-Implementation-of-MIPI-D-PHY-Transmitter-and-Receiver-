# Design-and-Implementation-of-MIPI-D-PHY-Transmitter-and-Receiver-

## Overview
This project involves the RTL design, implementation, and verification of a **MIPI D-PHY** Transmitter and Receiver, compliant with the MIPI D-PHY v1.2 standard, with enhancements from v2.5 for improved performance. The D-PHY is a key physical layer used in camera (CSI-2) and display (DSI) interfaces, supporting both High-Speed (HS) data transmission and Low-Power (LP) signaling.

The design covers:
- High-Speed data serialization and transmission
- Low-Power signaling control
- FSM (Finite State Machine) for HS/LP mode transitions
- PRBS-9 based data calibration and testing
- Functional verification with SystemVerilog Testbenches

## Directory Structure


## Features
- **High-Speed (HS) Transmission:** Parallel-to-serial data conversion for fast signaling.
- **Low-Power (LP) Transmission:** Control signals in LP mode with proper state handling.
- **State Machine Control:** Accurate HS entry/exit sequences following MIPI D-PHY standard.
- **PRBS-9 Calibration:** Pseudorandom bit sequences for data pattern testing and validation.
- **Full Verification:** Modular SystemVerilog testbenches to verify each RTL component individually.

## How to Run
1. **Prerequisites:**  
   - Simulator: ModelSim, VCS, or any SystemVerilog-compatible simulator.
   
2. **Simulation Steps:**
   ```bash
   cd TB
   # Example: simulate DPHY_HSTX
   vsim DPHY_HSTX_TB.v
