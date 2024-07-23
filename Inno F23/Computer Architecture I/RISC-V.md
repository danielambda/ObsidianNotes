---
tags:
  - CompArch
---
- Developed in University of California, Berkeley since 2010 -
- Reduced instruction set computer ([[RISC and CISC|RISC]]) ISA 
- Maintained by RISC-V International Foundation 
- Has 32 registers (from x0 to x31)
- Instructions size is 32 bits, and registers size is 64 bits 
- Supports 32, 64, and 128 bits memory addressing 
- Used in consumer electronics, network/storage equipment, cameras, printers, etc. 
- RISC-V is the natural successor to MIPS (the development of which in turn has been recently stopped)
## Naming Conventions
![[Pasted image 20231004184910.png]]
## Arithmetic Example
- C code:
``` C
f = (g + h) - (i + j);
```
- RISC-V code (ABI naming for registers)
``` RISC-V
add t0, g, h  # temp t0 = g + h 
add t1, i, j  # temp t1 = i + j 
sub f, t0, t1 # f = t0 − t1
```
## Instructions for bitwise manipulations
![[Pasted image 20231004190702.png]]
## Complicated Example
![[Pasted image 20231004190753.png]]
## Loop Example
![[Pasted image 20231004190817.png]]
## Floating-Point Registers
- RISC-V uses separate Floating-Point Registers for ALU float instructions
	- Unlike [[MIPS]], which uses separated Floating-Point Coprocessor  