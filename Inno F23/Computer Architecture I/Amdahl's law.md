---
tags:
  - CompArch
---
## Definition
- Amdahl's law can be formulated in the following way: $$S_{latency}(s) = \frac{1}{(1-p)+p/s}$$
	where:
	- $S_{latency}$ is the theoretical speedup of the execution of the whole task
	- $s$ is the speedup of the of the part of the task that benefits from improved system resources
	- $p$ is the proportion of execution time that the part benefiting from improved resources originally occupied
### Furthermore
$\left\{\begin{split} S_{latency}(s) \leq \frac{1}{1 - p} \\ \displaystyle\lim_{s\to\infty}S_{latency}(s) = \frac{1}{1 - p} \end{split}\right.$

- Amdahl’s law provides a theoretical upper bound on the execution speedup thanks to the parallelization of a program execution 
- Aspects to consider: 
	- Some program instructions depend on the execution result of a previous instruction
	- Some other instruction does not depend on the execution result of a previous instruction
	- Instructions, which do not depend on the previous instruction, can be executed in parallel with a previous instruction
## Interpretation
- Consider some program
- Let $x\%$ of instructions depend on the execution result of a previous instruction
- Other $(100 - x)\%$ do not depend 
- In case we execute those $(100 − x)\%$ instructions upon m processors in parallel, it will be $m$ times faster than on 1 processor Amdahl’s law characterizes the resulted speed-up gain of m processors over one processor: $$\large speedup = \frac{t_{onePocessor}}{t_{mProcessprs}} = \frac{1}{x + \frac{1-x}{m}}$$
![[Pasted image 20231004130848.png]]
