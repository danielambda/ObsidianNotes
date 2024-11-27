---
id: Hypergeometric Distribution
aliases: []
tags: []
---

## Intuition + Definition
- Hypergeometric Distribution can be described as fitting into the following generic scheme:
	- There are $N$ tickets in a bag, of which $b$ are "good" tickets, and $N-b$ are "bad". You draw $n$ tickets one by one (without putting them back). Let $\xi$ be the number of good tickets that you drew.
- A simpiale combinatorics gives: $$
	\mathbb R (\xi = x) = \frac{C_b^x C_{N-b}^{n-x}}{C_N^n}I(x\in\set{0, 1, \dots, n})
$$
- with understanding that $\forall \beta > \alpha: C_\alpha^\beta = 0$

## [[Expected Value]]
- Can be obtained via its [[Linearity]]. We can consider $\xi$ to be the sum of [[Indicator Function]]s: $$\xi = I_1+\dots+I_b$$
- All $I$'s have the same probability to by $1$, which gives $\mathbb E I_j= \displaystyle \frac{n}N$. Therefore $$\mathbb E\xi = \sum_{j=1}^b \mathbb E I_j = \frac{bn}N$$

## Second Moment $\mathbb E \xi^2$
$$
\mathbb E \xi ^2 = \mathbb E\left(\sum_{j=1}^b I_j\right)^2 = \sum_{j=1}^{b}
$$
