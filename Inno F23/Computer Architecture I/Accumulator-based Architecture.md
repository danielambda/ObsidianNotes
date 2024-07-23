---
tags:
  - CompArch
---
## Definition
- Single register A
- One explicit operand per instruction 
- Two instruction types: op (A := A op \*M) and load/store (\*M := A) 
- Short instructions possible, minimal internal state 
- High memory traffic – many loads and stores
## Example 
The code segment for $C = A+B$
```
Load A
Add B
Store C
```
## Advantages
- Minimizes internal state of machine
- Short instructions
## Disadvantages
- Since accumulator in only temporary storage, memory traffic is high