---
tags:
  - Math
  - MathematicalAnalysis
  - DifferetialForms
---
## Definition
- Hodge operator ($\star$) is a [[Linearity|linear]] operator, such that
$$\star:\Lambda^m(\mathbb R^n)\to\Lambda^{n-m}(\mathbb R^n)$$
$$\star dx_I=dx_J, \text{such that } dx_I\wedge dx_J=dx_1\wedge...\wedge dx_n$$
## Example 
$$\omega=dx_1\wedge dx_2+2dx_3\wedge dx_4+7dx_1\wedge dx_5$$
$$\star\omega=\star (dx_1\wedge dx_2)+2\star(dx_3\wedge dx_4)+7\star(dx_1\wedge dx_5)=$$$$=
dx_3\wedge dx_4\wedge dx_5+2dx_1\wedge dx_2\wedge dx_5-7dx_2\wedge dx_3\wedge dx_4$$