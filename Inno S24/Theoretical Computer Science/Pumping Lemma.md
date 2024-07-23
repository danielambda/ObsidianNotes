---
tags:
  - Math
  - TCS
---
## Lemma
- Given a [[Regular Language]] $L$, if $x\in L\;\&\;|x|\geq|Q|$, then there exists a $q\in Q\;\&\; w\in I^+$ such that:
	- $x=ywz$
	- $\delta^*(q_0,y) = q$
	- $\delta^*(q,w)=q$
	- $\delta^*(q,z)=q'\in F$
	- $|yw|\leq Q$
	- $yw^nz\in L, n\in\mathbb N$
## Formally
- $\forall L \in$ [[Regular Language]]s$:\exists x\in L: |x|\geq|Q|\implies \exists q\in Q\;\exists w\in I^+:$ 
	- $x=ywz$
	- $\delta^*(q_0,y) = q$
	- $\delta^*(q,w)=q$
	- $\delta^*(q,z)=q'\in F$
	- $|yw|\leq Q$
	- $yw^nz\in L, n\in\mathbb N$
## Therefore
- Pumping lemma is necessary but not sufficient condition for [[Language in TCS]] to be a [[Regular Language]]
## Application
- Consider [[Language in TCS|language]] $L=\set{a^nb^n|n\in\mathbb N}$
- Is it a [[Regular Language]]?
- Consider $x=a^mb^m, m>|Q|$ and let us apply the [[Pumping Lemma]]
- Possible cases:
1.  $\large x=ywx, w=a^k, k>0\implies\forall r\in\mathbb N a^{m-k}\color{red}a^{r\cdot k}\color{white}b^m\in L$ - false
2.  $\large x=ywx, w=b^k, k>0\implies\forall r\in\mathbb N a^{m}b^{r\cdot k}\color{red}b^{m-k}\color{white}\in L$ - false
3.  $\large x=ywx, w=a^kb^s, k>0\implies\forall r\in\mathbb N a^{m-k}\color{red}(a^{k}b^s)^r\color{white}b^{m-s}\in L$ - false
## [[Contrapositive]] (Negation)
- $\forall L\in$ [[Regular Language]]s: $\forall x\in L: |x|\geq|Q|\lor \forall q\in Q\;\forall w\in I^+:$
	- At least one of the following is false
	- $x=ywz$
	- $\delta^*(q_0,y) = q$
	- $\delta^*(q,w)=q$
	- $\delta^*(q,z)=q'\in F$
	- $|yw|\leq Q$
	- $yw^nz\in L, n\in\mathbb N$
## Practical Formalization 
- $L\in$ [[Regular Language]]s $\implies \exists m\in\mathbb N_+: \forall w\in L, |w|\geq m$ can be represented as $w=xyz$ such that:
	- $y\not=\varepsilon\;\&\; |xy|\leq m$  
	- $\forall r\in\mathbb N:xy^rz\in L$
## Practical [[Contrapositive]] (Negation)
- $\forall m\in\mathbb N_+\;\exists w\in L, |w|\geq m\;\&\; \forall$ representation $w=xyz, y\not=\varepsilon\;\&\; |xy|\leq m:$ $$\exists r\in\mathbb N_+: xy^rz\not\in L$$
- $\implies L$ is not a [[Regular Language]] 