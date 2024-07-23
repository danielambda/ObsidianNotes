---
tags:
  - CompArch
---
## Definition
- A stack machine has a stack as a part of the processor state 
- No registers
- No explicit operands in Instruction Set 
- Typical operations: push, pop, +, *, ...
- Instructions like + implicitly specify the top 2 elements of the stack as operands.
## Example
The code segment for $A = B + C  * D$
```
Push B; Push C; Push D
Mul
Add
Pop A
```
## Advantages
- Short instructions and easy to write compiler
- Simple model of expression evaluation
- Good code density
## Disadvantages
- Inefficient code and stack is a bottleneck
- Stack cannot be randomly accessed
- Makes it more difficult to generate efficient code.
- Results in the highest memory traffic during program execution