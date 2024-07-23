---
tags:
  - CompArch
---
## Definition
- Also called stored program computer (instruction in memory). 
### Key properties:
- Stored program
	- Instructions stored in a linear memory array (directly addressable!)
	- Memory is unified between instruction and data
		- The interpretation of a stored value depends on the control signals
- Sequential instruction processing
	- One instruction processed (fetched, executed, and completed) at a time
	- Program counter (instruction pointer) identifies the current instruction
	- Program counter is advanced sequentially except for control transfer instructions
- Other architectures are available, including [[Harvard Architecture|Harvard]]
## !!
- All major instruction set architectures today use Von-Neumann model (with minor variations, such as separate instruction and data caches, and multi-core clusters). 
	- For example: x86, ARM, RISC-V, SPARC, Alpha, POWER...
- At the microarchitecture level the execution model of almost all implementations is very different. Features of some microarchitectures: 
	- Pipelined instruction execution: Intel 80486
	- Multiple instructions at a time: Intel Pentium
	- Out-of-order execution: Intel Pentium Pro
	- Separate instruction and data caches 
- But, what happens underneath and is not consistent with the von Neumann model is not exposed to software 
## An Oversimplified Computer Organization
Consists of:
- [[The Control Unit]]
- [[The Arithmetic and Logic Unit]]
- [[Registers]]
- [[Communication Bus]]
- [[Main Memory]]
- [[Disk Storage]]

![[An Oversimplified Computer Organization.png]]
