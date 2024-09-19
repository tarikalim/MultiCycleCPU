
# 8-bit CPU Design

This project involves the design and implementation of a simple multi-cycle 8-bit central processing unit (CPU). The CPU design includes various subcircuits such as registers, an Arithmetic Logic Unit (ALU), and a control unit. The project was developed using **Logisim**, a digital logic simulator.

## Project Overview
The CPU is designed to handle basic operations including:
- **mv**: Move data between registers
- **mvi**: Move immediate data to a register
- **add**: Add values from two registers
- **sub**: Subtract values from two registers

The CPU is comprised of the following components:
- **8 Registers** that can each store 8-bit data
- **ALU** capable of performing addition and subtraction
- **Control Unit** that manages the execution of the operations
- **Counter** to track the time steps and manage multi-cycle instructions
- **ROM (Read-Only Memory)** to store and quickly execute instructions

## Implementation
The design leverages subcircuits to create a streamlined and modular CPU architecture. The key components include:
- **Registers Subcircuit**: Handles the storage and transfer of 8-bit data
- **Multiplexer (MUX) Subcircuit**: Directs data between different parts of the CPU
- **ALU Subcircuit**: Performs arithmetic operations such as addition and subtraction
- **Control Unit Subcircuit**: Manages the overall operation of the CPU
- **Counter**: Tracks the clock cycles, used in multi-cycle instruction execution

## Instruction Set Architecture (ISA)
The CPU is designed to execute a simple instruction set with operations encoded in machine code. Instructions are stored in the ROM and can be executed quickly during operation. Some of the key instructions include:
- **mvi**: Move immediate data to a register
- **add**: Add values from two registers and store the result
- **sub**: Subtract one register value from another

## Results
- At the end of execution, register **R5** contains `(B7)16` and register **R6** contains `(27)16`.
- The ALU was used to perform subtraction operations and the results were successfully stored in the registers.
- The CPU design successfully handles all operations within 18 clock cycles.

## Discussion
- The design is fully functional for the given instruction set but could be expanded for more complex operations in future iterations.
- A minor issue was noted with the Counter's reset system during certain operations like **mv** and **mvi**.
- The current design handles basic operations within 3 clock cycles without needing additional reset logic, but future designs with more complex instructions may require a more advanced Counter reset system.

## Tools Used
- **Logisim**: Digital logic simulator used for the design and implementation of the CPU.

## Contribution
- **Tevfik Tarık Alim**: Circuit design and Control Unit design.
- **Abdullah Kiraz**: Assisted in the overall design.
- **Kaan Edip Özoğuz**: Resolved issues in the final stages of the design.

## Conclusion
This 8-bit CPU design successfully demonstrates basic multi-cycle CPU functionality, and with further modifications, it can handle more complex instructions. The modular structure ensures easy scalability and future expansion.

