---
tags:
  - Math
  - TCS
---
## Definition
- Let $T=<Q, \Sigma,\Gamma,\delta, q_0, Z_0, F>$ be a [[Turing Machine]], $s$ be a given string. The length of [[Sequence]] $c_0\vdash^*c_F$ is called a TIME-[[Function]]
$$\text{TIME}(T,s)$$
## f-time-computable
- Let $f$ be a [[Function]], $c$ be a constant. A [[Turing Machine]] is called $f$-time-computable, if $$\forall s\in L:\text{TIME}(T,s)\leq c\cdot f(|s|)$$
## P-time-computable
- Let $T$ be a deterministic [[Turing Machine]]. $T$ is called P-time-computable, if it is 
$$\exists n\in\mathbb N:x^n\text{-time-computable}$$
## NP-time-computable
- Let $T$ be a non-deterministic [[Turing Machine]]. $T$ is called NP-time-computable, if it is 
$$\exists n\in\mathbb N:x^n\text{-time-computable}$$
## Fact
- $P\subseteq NP$