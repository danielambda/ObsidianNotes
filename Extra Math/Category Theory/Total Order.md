---
tags:
  - Math
  - CategoryTheory
  - DiscreteMath
  - Logic
---
## Definition
- *Total Order* is a [[Binary Relation]] which is:
	- Composable
	- [[Associativity|Associative]]
	- [[Reflexivity|Reflexive]] 
	and 
	- $\forall a, b: aRb \implies \neg bRa$ (without this it is [[Preorder]])
	- $\forall a,b: aRb \lor bRa$ (without this it is a [[Partial Order]])

- So, every [[Preorder]] is a [[Partial Order]] and every [[Partial Order]] is a [[Total Order]]