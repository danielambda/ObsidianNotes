---
tags:
  - Math
  - TCS
---
## Definition
- Let $T=<Q,\Sigma,\Gamma,\delta,q_0,Z_0,F>$ be a [[Turing Machine]]. $s$ be a given string. The length of working space in tape for $s$ is a SPACE [[Function]]:
$$SPACE(T,s)$$
## f-SPACE-computable
- Let $f$ be a [[Function]], $c$ be a constant. [[Turing Machine]] is called $f$-space-computable if $$\forall s\in L:\text{SPACE}(T,s)\leq c\cdot f(|s|)$$
## PSPACE-computable
- Let $T$ be a deterministic [[Turing Machine]]. T is called PSACE-computable, if it is $$\exists n\in\mathbb N:x^n\text{-SPACE-computable}$$
## NPSPACE-computable
- Let $T$ be a non-deterministic [[Turing Machine]]. T is called PSACE-computable, if it is $$\exists n\in\mathbb N:x^n\text{-SPACE-computable}$$
## Theorem (Savitch, 1970)
$$\text{PSPACE}=\text{NPSPACE}$$