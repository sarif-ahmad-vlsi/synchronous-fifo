# synchronous-fifo
Synchronous FIFO design and functional verification using Verilog/SystemVerilog, covering full/empty flags, overflow/underflow, reset, read/write operations, and synthesis using Synopsys VCS, Verdi, and Design Compiler.

# Synchronous FIFO — RTL Design, Functional Verification & Synthesis
## 📌 Project Overview
This project focuses on the RTL design, functional verification, and synthesis of a parameterized Synchronous FIFO (First-In, First-Out) using Verilog/SystemVerilog.

A synchronous FIFO stores data temporarily and follows the First-In, First-Out principle: the first data written into the FIFO is the first data read out. Read and write operations are synchronized to the same clock.

The design is verified using simulation test cases and synthesized using Synopsys Design Compiler.

## 🎯 Project Objectives
- Design a parameterized synchronous FIFO using Verilog/SystemVerilog.
- Implement read and write operations synchronized to a common clock.
- Generate `full` and `empty` status flags.
- Handle reset, overflow, and underflow conditions.
- Verify normal and boundary-condition scenarios through simulation.
- Perform RTL synthesis using Synopsys Design Compiler.

## 🛠️ Tools & Technologies
- HDL: Verilog HDL / SystemVerilog
- Simulation: Synopsys VCS
- Waveform Debugging: Synopsys Verdi
- Synthesis: Synopsys Design Compiler
- Technology Library: 32 nm standard-cell library, as used in the synthesis setup

## ⚙️ Design Features
- Parameterized data width and FIFO depth
- Synchronous reset and clock-controlled operation
- Read and write pointer management
- Full and empty status flag generation
- Overflow and underflow condition handling
- Support for read, write, and simultaneous read/write requests

## 🧪 Verification Scenarios
The testbench is designed to check the following scenarios:
1. Reset and initialization
2. Writing data into the FIFO
3. Reading data in FIFO order
4. Full FIFO condition
5. Empty FIFO condition
6. Overflow attempt when the FIFO is full
7. Underflow attempt when the FIFO is empty
8. Simultaneous read and write operations
9. Boundary conditions involving FIFO capacity

## 🔄 Verification Workflow
1. Develop the FIFO RTL.
2. Create a testbench to apply read/write transactions.
3. Compile and simulate the design using Synopsys VCS.
4. Inspect simulation waveforms using Synopsys Verdi.
5. Check FIFO behavior, data ordering, and status flags.
6. Synthesize the RTL using Synopsys Design Compiler.

## 📁 Suggested Repository Structure
synchronous-fifo/
├── rtl/
│   └── synchronous_fifo.v
├── tb/
│   └── synchronous_fifo_tb.sv
├── sim/
│   └── simulation.log
├── synthesis/
│   └── synthesis_reports/
├── screenshots/
│   └── fifo_waveform.png
└── README.md

## 📊 Results
Include your verified results here after running simulation and synthesis.
- Functional simulation: Add the actual pass/fail result from your simulation log.
- FIFO data ordering: Document the observed result from your testbench.
- Full/empty flags: Record the verified behavior.
- Synthesis: Add actual area, timing, or cell statistics if available.

## 📚 Key Learnings
- FIFO architecture and pointer management
- Synchronous RTL design
- Functional verification of boundary conditions
- Simulation and waveform debugging
- RTL synthesis and report analysis

## 👨‍💻 Author
Sarif Ahmad 
M.Tech — Electronic Circuits and System Design  
Aligarh Muslim University (AMU)

- LinkedIn: https://www.linkedin.com/in/ahmad-a-68b500138/
- GitHub: https://github.com/sarif-ahmad-vlsi
