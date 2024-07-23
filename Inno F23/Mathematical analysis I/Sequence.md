---
tags:
  - Math
  - MathematicalAnalysis
---
## Definitions
- sequence in a function  $(x_n)_{n\in\mathbb N}: \mathbb N \to \mathbb R$, usually presented as $x_0, x_1, x_2, ...$
- $x\in\mathbb R$ is a [[Limit of a Sequence|limit]] of a sequence $(x_n)_{n\in\mathbb N}\iff x = \displaystyle\lim_{n\to\infty} x_n$

## Examples
T. $(1 - \frac{1}{n+1})_{n\in\mathbb N}$ has a [[Limit of a Sequence|limit]] 1
P. (by definition)
- Let $\varepsilon > 0 \in \mathbb R$
- Let $m \in\mathbb N$ be the first number such that $\frac{1}{m} \leq \varepsilon$
	- Then $\forall n\geq m\frac{1}{n}\leq\frac{1}{m}\leq\varepsilon$
	- $|1 - (1-\frac{1}{1+n})| = |(1-\frac{1}{1+n})| \leq \frac{1}{m}\leq\varepsilon$ 
	- $\implies$ is has a limit 1. $Q.E.D. \blacksquare$
## [[Subsequence]] 