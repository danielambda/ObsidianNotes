---
tags:
  - Math
  - TCS
---
## Theorem
- A [[Language in TCS|language]] $L$ is a [[Regular Language]] $\iff$ $\equiv_L$ has a finite number of [[Equivalence Class]]es
## $\equiv_L$ Relation
- For a [[Language in TCS|language]] $L$ over an [[Alphabet in TCS|alphabet]] $A$ $$s_1\equiv_L s_2\iff(\forall t\in A^*:s_1t\in L\iff s_2t \in L)$$
- $\equiv_L$ is an [[Equivalence Relation]] 
---
- For a [[Language in TCS|language]] $L$ over an [[Alphabet in TCS|alphabet]] $A$ $$s_1\not\equiv_L s_2\iff(\exists t\in A^* : s_1t\in L\not= s_2t\in L)$$
- $t$ is called a **distinguishing extension**