---
tags:
  - Math
  - Logic
---
## Definition
- We need to prove: $\forall n \geq \alpha_0:P(n)$
#### Induction Basis / Initial step
- Prove $P(1)$
#### Induction / Inductive Hypothesis
- Suppose that $P(k), k\geq \alpha_0$
#### Induction / Inductive step
- Prove $P(k + 1)$
#### Conclusion
- Therefore, by the Principle of [[Mathematical induction]] $\forall n\geq\alpha_0: P(n)$ 
### Formally
$$\begin{array}{l}P(\alpha_0)\\
\forall k\geq\alpha_0\;[P(k)\implies P(k + 1)]\\\hline \forall n\geq\alpha_0\;P(n)\end{array}$$
## [[Strong Induction in Formal Logic]]