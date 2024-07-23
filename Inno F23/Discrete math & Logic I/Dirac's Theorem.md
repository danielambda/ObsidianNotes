---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
slide: "12.70"
---
## Theorem
- Let $G$ be a simple [[Graph]] with $n\geq 3$ vertices.
- Suppose that for any vertex $v$ $$deg(v)\geq n/2$$
- Then $G$ is [[Hamilton Cycle|Hamiltonian]] 
## Proof
By [[Contradiction in Formal Logic|Contradiction]]
- Assume that $G$ is not [[Hamilton Cycle|Hamiltonian]]
- Let $G'\supseteq G$ be a maximal non-[[Hamilton Cycle|Hamiltonian]] with the same vertices.
- It means that $G'+vv'$ is [[Hamilton Cycle|Hamiltonian]] for any non-adjacent vertices $v,v'$
	- Note that $G'$ is not a complete [[Graph]]
- Choose some non-adjacent vertices $v,v'$
- Since $G'+vv'$ is [[Hamilton Cycle|Hamiltonian]], $G'$ contains a [[Hamilton Path]] from $v$ to $v'$
1. Suppose that there exists $i (1<i<n)$ such that $vv_i\in G'\;\&\;v_{i-1}v'\in G'$
	- Hence $v_1...v_{i-1}v_nv_{n-1}...v_iv_1$ is a [[Hamilton Cycle]]
	- This is a [[Contradiction in Formal Logic|Contradiction]], $\square$
2. Suppose that there does not exist $i(1<i<n)$ such that $vv_i\in G'\;\&\;v_{i=1}v'\in G'$
	- Let $D_1(v)=\{v_i|vv_i\in E'\}$ and $D_2(v')=\{v_i|v_{i-1}v'\in E'\}$
	- $\implies D_1(v)\cap D_2(v')=\emptyset$
	 - $v_1v_n\not\in E'\implies |D_1(v)\cup D_2(v')|<n$
	 - Therefore, $deg(v)+deg(v')<n$
	 - This is a [[Contradiction in Formal Logic|contradiction]] with $\forall u\in V:deg(u)\geq n/2$