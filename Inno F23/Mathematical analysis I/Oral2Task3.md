---
tags:
  - Math
  - MathematicalAnalysis
---
$M = 25 + 10 = 35$

---
## Task
- Does $(n-\frac{M}{n+1})_{n\in\mathbb N}$ have a real limit? Prove your answer using [[Cauchy Sequences Convergence test]].
## Solution
### Answer:
- No, it does not
### Proof:
- Let $x_n=n-\frac{M}{n+1}$
[[Cauchy Sequences Convergence test]]: $$\forall\varepsilon\in\mathbb R, \varepsilon>0\;\exists m\in\mathbb N\;\forall n_1, n_2\geq m: |x_{n_1}-x_{n_2}| \leq \varepsilon$$
- Sequence does not meat [[Cauchy Sequences Convergence test]] means:
$$\exists\varepsilon\in\mathbb R, \varepsilon>0\;\forall m\in\mathbb N\;\exists n_1,n_2\geq m: |x_{n_1}-x_{n_2}|>\varepsilon$$
- We need to find real number $\varepsilon>0$ such that for every natural numbers $m$ there are two natural numbers $n_1, n_2$ that are greater or equal to $m$ such that it is true that $|x_{n_1}-x_{n_2}| > \varepsilon$ 
- Let $\varepsilon = 1, n_2=n_1+2$ 
$$|x_{n_1}-x_{n_2}|=\left|\left(n_1-\frac{M}{n_1+1}\right)-\left(n_2-\frac{M}{n_2+1}\right)\right|=$$
$$=\left|\left(n_1-\frac{M}{n_1+1}\right)-\left((n_1+2)-\frac{M}{(n_1+2)+1}\right)\right|=$$
$$=\left|n_1-\frac{M}{n_1+1}-n_1-2+\frac{M}{n_1+3}\right|=\left|-\frac{M}{n_1+1}-2+\frac{M}{n_1+3}\right|=$$
$$=\left|2+\frac{M}{n_1+1}-\frac{M}{n_1+3}\right|$$
- Since $\displaystyle n_1+1<n_1+3\implies \frac{M}{n_1+1}>\frac{M}{n_1+3}\implies\frac{M}{n_1+1}-\frac{M}{n_1+3}>0$ 
$$\left|2+\left(\frac{M}{n_1+1}-\frac{M}{n_1+3}\right)\right|>|2|=2>1=\varepsilon$$
- To sum up, we got that $$n_2=n_1+2\implies|x_{n_1}-x_{n_2}|>\varepsilon$$
- Let us take $n_1=m, n_2=n_1+2=m+2$
- Now for every $m$ we have $n_1, n_2$ such that $|x_{n_1}-x_{n_2}|>\varepsilon, Q.E.D.\blacksquare$