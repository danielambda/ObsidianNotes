---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
slide: "14.6"
aliases:
---
## Definition
*Flow* in a [[Transportation Network]] $N=(V,E,c,s,t)$ is a [[Function]] $f:E\to\mathbb R^+$ such that:
1. $\forall e\in E:0\leq f(e)\leq c(e)$
2. $\displaystyle\sum_{w\in V}f\overline{(v,w)}=\sum_{w'\in V}f\overline{(w',v)}$
---
- the value of flow $f$ is $\displaystyle\sum_{w\in V}f\overline{(s,w)}$
## [[Ford-Fulkerson Algorithm]]