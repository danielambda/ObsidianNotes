---
tags:
  - Math
  - SetTheory
  - Logic
---
## Definition 
- $Y$ is a binary relation on $X_1, X_2$ if $X$ is a Cartesian product of sets $X_1, X_2$ (i.e., $Y \subseteq X_1 \times X_2$)
## Properties
- reflexive $\iff \forall x: xRx \equiv true$
- irreflexive $\iff \forall x: xRx \equiv false$
- symmetric $\iff \forall x, y:(xRy \iff yRx)$
- asymmetric $\iff(\forall x,y:(xRy\implies\neg yRx))\iff(\forall x,y: \neg(xRy\;\&\;yRx))$
- anti-simmetric $\iff \forall x,y:(xRy\;\&\;yRx\implies x=y)$
- transitive $\iff \forall x, y, z: (xRy\;\&\;yRz) \implies xRz$
- connex $\iff \forall x,y:(xRy\lor yRx)$