# RISC-V 5-Stage Pipelined-Processor

This project implements a **RISC-V 5-Stage Pipelined Processor**. It includes five key stages: **Instruction Fetch (IF)**, **Instruction Decode (ID)**, **Execution (EX)**, **Memory Access (MEM)**, and **Write Back (WB)**. The architecture demonstrates how instruction execution is divided into parallel stages to improve throughput and processor performance.

**Note**: Hazards (data, control, and structural) have not been handled in this implementation. 

## Features
- **5-Stage Pipeline**: Includes the stages IF, ID, EX, MEM, and WB for executing instructions.
- **Parallel Execution**: Increases instruction throughput by executing multiple instructions simultaneously across different pipeline stages.
- **Basic RISC-V Components**: Includes an ALU, registers, memory, and a control unit for instruction processing.

# Prerequisites

To set up and work on this project, the following tools and libraries are required:
### SystemVerilog: 
For designing and implementing the processor.
### VSCode: 
Recommended for editing and managing the SystemVerilog files.
### GTKWave: 
For waveform visualization (requires Multisim for functionality).
### Simulator: 
Tools like ModelSim or Vivado for simulation and testing.

# Commands To use 
```
vlog *.sv
vsim -c tb_processor -voptargs=+acc -do "run -all"
gtkwave processor.vcd
```
