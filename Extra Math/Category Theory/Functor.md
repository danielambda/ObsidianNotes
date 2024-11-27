---
id: Functor
aliases: []
tags:
  - Math
  - CategoryTheory
  - Programming
---
## Definition
- *Functor* is a structure preserving [[Map]] from one [[Category]] to another (including itself)
- For [[Category|Categories]] $C$ and $D$ [[Map]] $C\to D$ is a *Functor* if:
	- $\forall a,b\in C:FC(a,b)=D(Fa,Fb)$
	- $\forall f\in C(a,b), g\in C(b,c): F(g\circ f)=Fg\circ Ff$
	- $F id_a=id_{Fa}$
