---
tags:
  - Math
  - MathematicalAnalysis
---
$M = 25 + 10 = 35$

---
## Task
Does $\displaystyle\left(2 + \frac{(−1)^n M}{\sqrt n+1}\right)_{n\in\mathbb N}$ has a limit? Prove your answer using the definition of the sequence’ limit.
## Solution
### Answer:
- Yes, it does.
### Proof:
Let $x_n = \displaystyle\left(2 + \frac{(−1)^n M}{\sqrt{n+1}}\right)_{n\in\mathbb N}$
- Let us proof that $2$ is the limit of the given [[Sequence]]
- $2$ is the limit means $$\forall\varepsilon>0\;\exists m\in\mathbb N\;\forall n\geq m:|x_n-2|\leq\varepsilon$$
- For every $\varepsilon>0$ we need to find $m\in\mathbb N$ such that for every $n\in\mathbb N$ that is greater or equal to $m$, $\left|\displaystyle2 + \frac{(−1)^n M}{\sqrt{n+1}}-2\right|$ will be less or equal to $\varepsilon$
- $\left|\displaystyle2 + \frac{(−1)^n M}{\sqrt{n+1}}-2\right|=\left|\displaystyle\frac{(−1)^n M}{\sqrt{n+1}}\right|$ since $M$ and $\sqrt{n+1}$ are non-negative numbers, equals to $\displaystyle\frac{M}{\sqrt{n+1}}$ $$\frac{M}{\sqrt{n+1}}\leq\varepsilon\iff\frac{M}{\varepsilon}\leq\sqrt{n+1}\iff\frac{M^2}{\varepsilon^2}-1\leq n$$
- Therefore, $\displaystyle m = \left\lceil\frac{M^2}{\varepsilon^2}\right\rceil$ will satisfy the conditions for $2$ to be a [[Limit of a Sequence]] $x_n, Q.E.D. \blacksquare$ 
## Wrong Solution
### Wrong Answer:
- No, it does not.
### Wrong Proof:
Let $x_n = \displaystyle\left(2 + \frac{(−1)^n M}{\sqrt{n+1}}\right)_{n\in\mathbb N}$
If [[Sequence]] $x_n$ does not have a limit, then $$\forall x\in\mathbb R\;\exists\varepsilon>0\;\forall m\in\mathbb N\;\exists n\geq m:|x-x_n|>\varepsilon$$$$\iff\forall x\in\mathbb R\;\exists\varepsilon>0\;\exists n:|x-x_n|>\varepsilon$$
- We need to find $\varepsilon>0$ for all real numbers such that there is a natural number $n$ such that $|x-x_n|>\varepsilon$ 
- Let us fix number $x\in\mathbb R$ 
- *И тут я понял, что я дурак, потому что последовательность-то сходится* 
- Эта часть была написана до правильного решения actually