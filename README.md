# RISC Processor (MIPS-32 Subset) – SystemVerilog | UVM | Verilator | GTKWave

This repository contains the design and verification of a **RISC processor** based on a **subset of the MIPS-32 ISA**, fully implemented using **SystemVerilog** and verified using **UVM**.  
The project includes a **five-stage pipelined microarchitecture** with hazard handling and a complete UVM-based verification environment.

---

## 🚀 Project Overview

### ✔️ Processor Architecture
- Implements a **subset of MIPS-32 ISA**  
- RISC-optimized datapath including:
  - ALU  
  - Register File  
  - Control Unit  
  - Data & Instruction Memory  
  - Multiplexers and supporting datapath components  
- Fully functional **5-stage pipeline**:
  1. IF – Instruction Fetch  
  2. ID – Instruction Decode  
  3. EX – Execute  
  4. MEM – Memory Access  
  5. WB – Write Back  

### ✔️ Hazard Handling
- **Data Hazards**
  - Forwarding / Bypassing
  - Load-use stall mechanism
- **Control Hazards**
  - Flush mechanism on taken branch

---

## 🧪 Verification (UVM)

A complete **UVM testbench** was developed to validate the processor pipeline.

### Testbench Features
- Constrained-random instruction generation  
- Coverage-driven verification  
- Scoreboard for reference result checking  
- Monitors & subscribers to track pipeline behavior  
- Assertions for protocol and timing checks  

### Tools Used
- **UVM 1.2**
- **Verilator** (compilation + simulation)
- **GTKWave** (waveform analysis)

---

