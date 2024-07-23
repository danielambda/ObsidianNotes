---
tags:
  - CompArch
a.k.a.: Instruction Pointer
---
## Definition
*Program Counter* (PC) register – the register containing the index/address of a program instruction being executed by a processor at a current time (or of the next instruction to be executed)
## PC-relative addressing
This mode can be used to load a register with a value stored in program memory Target address = PC + offset × 4 (each RISC-V instruction takes 4 bytes) PC already incremented by 4 by this time
## PC in CPU circuit design

![[Pasted image 20231031132937.png]]
