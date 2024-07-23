---
tags:
  - Math
  - Arithmetic
  - DiscreteMath
---
## Definition
- $S(n) = a_0+(a_0+d)+(a_0+2d) + ... + (a_0+nd)$
## Theorem
- $\displaystyle S(n) = \sum^n_{i=0}(a_0 + id) = (n+1)a_0+d\frac{n(n+1)}{2} =$
$\displaystyle=\frac{2a_0+dn}{2}(n+1) =$
$\displaystyle=\frac{a_0+a_n}{2}(n+1)$
## Proof
$\displaystyle \sum^n_{i=0}(a_0+id) = \sum^n_{i=0}a_0+\sum^n_{i=0}id=$
$=\displaystyle a_0\sum^n_{i=0}1+d\sum^n_{i=0}i = (n+1)a_0+d\frac{n(n+1)}{2} = \frac{2a_0+nd}{2}(n+1), Q.E.D.\blacksquare$