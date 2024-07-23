---
tags:
  - CompArch
---
## Definition
- Execution time for program $X$: $$ExecutionTime_X = ClockCycles_X\times CycleTime_{CPU}$$
- Alternatively: $$ClockRate_{CPU}=\frac{1}{CycltTime_{CPU}}; ExecutionTime_X = \frac{ClockCycles_X}{ClockRate_{CPU}}$$
## Important
- Different Instructions require different # of Cycles
## Vocabulary
- Cycle time (seconds per cycle)
- Clock rate (cycles per second)
- CPI (*average* cycles per instruction)
- MIPS (millions of instructions per second)
## Classic Equation
$$CPUtime = InsructionCount\times CPI\times ClockCycleTime$$$$\iff$$$$CPUtime = \frac{InstructionCount\times CPI}{ClockRate}$$