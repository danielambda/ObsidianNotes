---
tags:
  - Math
  - MathematicalAnalysis
slide: "3.57"
a.k.a.: Lagrange Theorem, Теорема Лагранжа
---
## Statement 
Each [[Continuity of a Set of Points|continuous]] on a closed finite interval $[a,b]$ function $f$ that
- is [[Differentiability on a Set of Points|differentiable]] in each interval point of the interval
has [[Derivative]] equals $\frac{f(b)-f(a)}{b-a}$ at some point of the interval
## Proof
- Let $\displaystyle g=\lambda x\in[a,b]. \left(f(x)-\left(\frac{f(b)-f(a)}{b-a}(x-a)+f(a)\right)\right)$
- $g\in C[a,b], g\in C^1[a,b], g(a)=g(b)=0$
- $\displaystyle g'=\lambda x\in(a,b).\left(f'(x)-\frac{f(b)-f(a)}{b-a}\right)$
- According to [[Rolle's Lemma]]: $$\displaystyle\exists c\in[a,b]: g'(c)=0\implies f'(c)=\frac{f(b)-f(a)}{b-a}, Q.E.D. \blacksquare$$
