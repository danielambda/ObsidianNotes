---
tags:
  - Math
  - MathematicalAnalysis
slide: "3.59"
russian: Формула Ньютона-Лейбница
---
## Statement
- Let $]a,b[$ be any open interval (may be infinite) and $f:]a,b[\to\mathbb R$ be a [[Continuity|continuous]] total real [[Function]]. Then:
	- the [[Indefinite Integral]] $\int f(x)dx$ exists
	- $\forall F\in\int f(x)dx\;\forall c,d\in]a,b[:\exists \int_c^df(t)dt:$ $$\Large\int_c^df(t)dt=F(d)-F(c)=F(x)\bigg\vert^{x=d}_{x=c}$$
## Proof 
- $r\in]a,b[\implies S=\lambda x\in]a,b[.\int_r^xf(t)dt$ is an [[Antiderivative]] for $f$.
- According to [[Indefinite Integral|additivity]]: $\int_c^df(t)dt=S(d)-S(c)$
- Since difference between any two [[Antiderivative|antiderivatives]] is a some "constant" value $C$ then: $$\int_c^df(t)dt=S(d)-S(c)=(F(d)+C)-(F(c)+C)=F(d)-F(c). \blacksquare$$