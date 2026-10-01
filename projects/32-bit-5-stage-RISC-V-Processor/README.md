# 32-bit 5-Stage RISC-V Processor

## Project Overview

A 32-bit pipelined RISC-V processor project focused on RTL design, processor datapath organization, pipeline control, hazard handling, forwarding, simulation, and FPGA implementation.

> **Repository status:** Project documentation is prepared here. The actual Verilog source, testbench, waveforms, and synthesis results should be added from the working project files.

## Architecture

```text
IF → ID → EX → MEM → WB
```

- **IF:** Instruction Fetch
- **ID:** Instruction Decode and Register Read
- **EX:** ALU / Branch Execution
- **MEM:** Data Memory Access
- **WB:** Register Write Back

## Main RTL Blocks

```text
Instruction Memory
       ↓
Program Counter
       ↓
IF/ID
       ↓
Instruction Decode ──→ Control Unit
       ↓
Register File
       ↓
ID/EX
       ↓
ALU ← Forwarding Unit
       ↓
EX/MEM
       ↓
Data Memory
       ↓
MEM/WB
       ↓
Register File
```

## Key Design Areas

- 32-bit processor datapath
- Five-stage pipelining
- Pipeline registers
- ALU and control logic
- Register file
- Immediate generation
- Instruction and data memory
- Data forwarding
- Hazard detection
- Branch handling
- RTL simulation
- FPGA implementation

## Verification Flow

```text
Verilog RTL
    ↓
Testbench
    ↓
Simulation
    ↓
Waveform Analysis
    ↓
Functional Verification
```

## Implementation Flow

```text
RTL
 ↓
Synthesis
 ↓
Implementation
 ↓
Timing Analysis
 ↓
FPGA Bitstream
```

## Results

Actual measurements should be added after the project files are uploaded.

| Metric | Result |
|---|---|
| Data width | 32-bit |
| Pipeline stages | 5 |
| HDL | Verilog |
| Simulation | Add actual tool |
| FPGA device | Add actual device |
| Maximum frequency | Add measured result |
| LUT usage | Add measured result |
| FF usage | Add measured result |

## Planned Repository Structure

```text
rtl/
tb/
simulation/
fpga/
docs/
README.md
```

## Skills Demonstrated

`Verilog HDL` · `RTL Design` · `Pipelined Architecture` · `Hazard Handling` · `Forwarding` · `Functional Verification` · `FPGA`

## Author

**Suriyaprakash N**

Electronics and Communication Engineering
