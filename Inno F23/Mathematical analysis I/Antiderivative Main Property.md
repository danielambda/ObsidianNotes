---
tags:
  - Math
  - MathematicalAnalysis
slide: "4.15"
---
## Statement
- Each constant [[Function]] $F=\lambda x\in]a,b[.const$ is an [[Antiderivative]] of an identical zero [[Function]] $f=\lambda x\in]a,b[.0$
- Each [[Antiderivative]] of any identical zero [[Function]] $f=\lambda x\in]a,b[.0$ is some $const$ function $F=\lambda x\in]a,b[.const$
- A difference between any two [[Antiderivative|Antiderivatives]] of a [[Function]] is a constant [[Function]]: 
$$F_1'=F_2'=f\implies F_1-F_2=\lambda x\in]a,b[.const$$
## Proof 
- Let $F$ be any [[Antiderivative]] of identical zero function $f=\lambda x\in]a,b[.0$ and $c,d\in]a,b[$ be any two point in the interval
- According to the [[Mean Value Theorem]]$$\exists t\in [c,d]:F(d)-F(c)=F'(t)\times(d-c)$$
- $F'(t)=f(t)=0\implies F(d)=F(c)\implies F=\lambda x\in ]a,b[.c$