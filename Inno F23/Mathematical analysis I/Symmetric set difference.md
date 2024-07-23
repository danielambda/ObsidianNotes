---
tags:
  - Math
  - SetTheory
---
## Definition
$X\Delta Y = \{z \in X\cup Y: (z \in X\lor z \in Y)\;\&\;\neg(z\in X\;\&\; z\in Y)\}$ 
## Prove that $X\Delta Y$ is a set №1
- From [[Union]] we know that $X\cup Y$ is a set. Let $X\cup Y = W$
- Let us construct $A$ from $W$ using specific properties: $$A = \{z \in W: \neg(z\in X \;\&\; z\in Y)\}$$
- From [[Naive Set Theory axioms]] $A$ is a  set, because $A$ is a specified subset of $W$
## Prove that $X\Delta Y$ is a set №2
- By definition: $X\Delta Y = \{z: (z \in X \lor z\in Y)\;\&\;\neg(z\in X\;\&\;z\in Y)\}$
- $Ж = X\cup Y$. It is proven that $Ж$ is a set ([[Union]])
- $X\Delta Y = \{z: (z \in X \lor z\in Y)\;\&\;\neg(z\in X\;\&\;z\in Y)\} =$ $= \{z \in Ж: (z \in X \lor z\in Y)\;\&\;\neg(z\in X\;\&\;z\in Y)\}$ 
- $X\Delta Y$ is a subset of $Ж$ specified by properties $\implies$ it is a set. $Q.E.D.\blacksquare$
