---
tags:
  - CompArch
---
## Definition
- All operands are explicit either registers or memory locations 
- General Purpose Registers (GPR) 
- Allows fast access to temporary values 
- Permits clever compiler optimization 
- Reduce traffic to memory
## Example
The code segment for $C = A+B$
```
load t0, A
loar t1, B
add s0, t0, t1
```

- Modern dominant architectures are Intel x86, ARM, RISC-V
## Advantages
- Most general model for code generation and the most common used model nowadays
## Disadvantages
- All [[Operand|operands]] must be named, leading to longer instructions