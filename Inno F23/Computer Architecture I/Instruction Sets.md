---
tags:
  - CompArch
---
## Definition
- the vocabulary of computer’s language, e.g. RISC-V or Intel x86 instruction sets:
	- Instruction set includes a complete set of instructions, recognizable by a given hardware platform 
	- Different computers have different instruction sets, but many aspects are similar 
	- Early computers had very simple instruction sets, to support a simple hardware implementation 
	- Many modern computers also have simple instruction sets
## Classification
- The instruction sets can be classified by:
	- Number of addresses (1, 2, 3, ...)
	- [[Operand]] internal storage inside the CPU
	- Number of explicit operands per instruction
	- Operand location
	- Operations
	- Type and size of operands
- The type of internal storage in the CPU is the most basic differentiation. The major choices are:
	- [[Stack-based Architecture]]
	- [[Accumulator-based Architecture]]
	- [[Register-based Architecture]]
![[Pasted image 20231004183910.png]]

## Historical facts
- The earliest machines used stack or accumulator-style architectures
- In the past twenty years, all machines use register-set based architecture (except quantum)
- The reasons for using register-based architecture: 
	- Registers are faster than RAM memory 
	- Allows sophisticated optimizations during program compilation 
	- Other
## Examples
- add $a, b, c : a + b \to c$