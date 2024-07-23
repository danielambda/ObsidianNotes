---
tags:
  - Math
  - TCS
  - Algorithms
---
## This is an
- algorithm to get [[Regular Expression]] from [[Finite State Automaton (FSA)]]
## Algorithm
### Intuitively
#### Union

#### Concatenation
![[Pasted image 20240404145503.png]]
#### [[Kleene Star]]
![[Pasted image 20240404145528.png]]

### Formally
- Let $M=<Q, A, \delta, q_0, F>$ be an [[Finite State Automaton (FSA)|FSA]], where $Q=\set{q_0,...,q_n}$
#### Step $k = -1$
$$\large R_{ij}^{-1}=\begin{cases}
a_1|...|a_m, \text{if $i\not=j$, where $\delta(q_i, a_t)=q_j$}\\
a_1|...|a_m|\varepsilon,\text{if $i=j$, where $\delta(q_i,a_t)=q_j$}\\
\emptyset, \text{otherwise}
\end{cases}$$
#### Step $k=0,...,n$
$$\large R_{ij}^k=R_{ik}^{k-1}\left(R_{kk}^{k-1}\right)^* R_{kj}^{k-1}|R_{ij}^{k-1}$$
#### Answer
$$\large R_{0i_1}^n|...|R_{0i_f}^n,\text{where } \set{q_{i_1},\dots,q_{i_f}}=F\text{ is the set of accept states}$$
#### Description
- Given an [[Finite State Automaton (FSA)|FSA]] $M$ 
	- $R_{ij}^k$ are the sets of all strings that take $M$ from state $q_i$ to $q_j$ without going through any state numbered lower than $k$
	- Each set $R_{ij}^k$ is represented by a [[Regular Expression]]
	- The algorithm computes $R_{ij}^k$ step by step for $k=[-1..n]$
	- Since there is no state numbered higher than $n$, the [[Regular Expression]] $R_{0j}^n$ represents the set of all strings that take $M$ from its start state $q_0$ to $q_j$
		- If $F=\set{q_{i_1},\dots,q_{i_f}}$ is the set of all final states, the [[Regular Expression]] $R_{0_{i_1}}^n|\dots|R_{0 i_f}^n$ represents the [[Language in TCS|language]] accepted by $M$
		