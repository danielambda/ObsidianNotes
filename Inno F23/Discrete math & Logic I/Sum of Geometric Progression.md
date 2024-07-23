---
tags:
  - Math
  - DiscreteMath
---
## Definition
- $S(n) = a_0+ta_0+t^2a_0+t^3a_0+...+t^na$
## Theorem
$\displaystyle S(n) = \sum^n_{i=0}(a_0t^i) = a_0\frac{t^{n+1}-1}{t-1}$
## Proof
- Let $S = \displaystyle\sum^n_{i=0}(a_0t^i) = a_0+ta_0+t^2a_0+...+t^na_0$
- Then $tS = ta_0+t^2a_0+t^3a_0+...+t^{n+1}a_0$
- $tS-S = t^{n+1}a_0-a_0$
- $S = \displaystyle\frac{t^{n+1}a_0-a_0}{t-1}=a_0\frac{t^{n+1}-1}{t-1}, Q.E.D. \blacksquare$
