---
tags:
  - CompArch
---
## Definitions
- For some program running on a machine $X$: $$Performance_X = \frac{1}{ExecutionTime_X}$$
- $X$ in $n$ times faster than $Y$, that is: $$\frac{Performance_X}{Performance_Y} = n$$
## Example
- Computer A executes a program in 20 seconds, while Computer B executes the same program in 25 seconds. How faster is Computer A than Computer B?
- Answer: 1.25 times
## Clock Cycles Usage
- We often use: $$\frac{seconds}{program} = \frac{cycles}{program} \times\frac{seconds}{cycle}$$
- The clock is a device which measures time
- The clock determines the sequencing of events
- Via clock cycles of constant time, also known as clock periods, clock ticks, or just ticks 
- The duration is called cycle time 
- The clock rate is $(tick)^{−1}$ Clock rate is the same as clock frequency. Clock generator: Generates the clock signal (e.g. rectangular waves) The clock signal is measured in Hertz (Hz) Note: Instructions to get a current clock cycle are available for different hardware platforms
## [[CPU Performance]]
## Factors
- Technology 
	- Circuit speed (clock, MHz) 
	- Processor technology 
- Organization 
	- Type of processor (ILP) 
	- Configuration of the memory hierarchy 
	- Type of I/O devices 
	- Number of processors in the system 
- Software
- Quality of the compilers 
- Organization and quality of OS, databases, etc