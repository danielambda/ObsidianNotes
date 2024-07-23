---
tags:
  - CompArch
---
- Arithmetic instructions use register operands
## Assembler names
- t0, t1, ..., t6 for temporary values
- s0, s1, ..., s11 for saved values
## Memory Operand Example
- C code:
``` C
g = h + A[8];
```
- Assumptions:
	- $A$ denotes an array, with each element of 1 word (4 bytes) in size
	- Variable $g$ is assigned to register $s1$, $h$ - to $s2$, and base address of $A$ - to $s3$
- Corresponding RISC-V code:
``` RISC-V
lw t0, 32(s3)
add s1, s2, t0
```
- Array element $A[8]$ requires offset of 32 bits for lw instruction 
- In RISC-V, words must start at addresses that are multiples of 4 
- This requirement is called an alignment restriction 
- Why? Because alignment leads to faster data transfers