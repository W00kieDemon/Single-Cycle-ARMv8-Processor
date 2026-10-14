# Single Cycle ARMv8 Overview
This repository aims to be a way to document the design workflow and implementation of my personal Single Cycle ARMv8 project. The ultimate goal of this project is to load a SystemVerilog implementation of a single cycle processor onto a FPGA; this processor should have the ability to display a text-based terminal that can display multiple programs in a hierarchical, folder format. This particular md file will provide a brief overview of my general design, future md files will go into further detail about specific module designs.

## Module Overview
This project aims to keep the processor as simple as possible while adhering to ARMv8/LEGv8 instruction language. This project will include 7 major modules. In no particular order, these modules are as follows:
- Control Unit
- Instruction Memory
- Register File
- Sign Extender
- Arithmetic Logic Unit (ALU)
- Data Memory
- Clock
 
