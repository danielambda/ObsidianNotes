---
tags:
  - Math
  - DataStructures
  - Algorithms
  - GraphTheory
  - Optimization
---
[[Flow in a Network]]
## Definition 
- A Flow Network $G=(V,E)$ is a directed [[Graph]] is which
	1. Each edge $(u,v)$ in $E$ has a non-negative *capacity* $c(u,v)\geq0$
	2. $(u,v)\in E\implies (v, u)\not\in E$
	3. $(u, v)\not\in E\implies c(u,v)=0$ by convention
	4. $(u,u)\not\in E$
	5. We have 2 distinguished vertices: *source* $s$ and *sink (target)* $t$
	6. Each vertex $u\in V$ is on path from $s$ to $t$
## Problem
- Given a flow network, we want to compute maximum flow: we want to find a way to utilize paths in the network in the most efficient way, achieving maximum throughput.
## Applications
1. Shipping/Logistics
2. Communication Networks
3. Bipartite Matching
4. Image Segmentation
5. And more...
## Flow trough a Flow Network
- Let $G=(V,E)$ be a flow network with capacity [[Function]] $c$, a source $s$ and sink $t$
- A flow in $G$ is a [[Function]] $f: $V\times V\to R$, such that
	1. $\forall u, v\in V: 0\leq f(u,v)\leq c(u,v)$
	2. $\forall u\in V/\set{s,t}\displaystyle\sum_{v\in V}f(u,v)=\sum_{w\in V}f(u,w)$
- $f(u,v)$ is a flow from $u$ to $v$
- Value of flow is $\displaystyle|f|=\sum_{v\in V}f(s,v)-\sum_{v\in V}f(v,s)$
## [[Ford-Fulkerson Algorithm]]
## Cuts
- A cut $(S,T)$ of network $G=(V,E)$ with source $s$ and sink $t$ is a partition of $V$ into $S$ and $T=V/ S$, such that $s\in S, t\in T$
#### Net flow across a cut
- (net flow) $\displaystyle f(S, T)=\sum_{u\in S}\sum_{v\in T} f(u,v) = \sum_{u\in S}\sum{v\in T} f(v,u)$
#### Capacity of a cut
- (capacity) $\displaystyle c(S,T)=\sum_{u\in S}\sum_{v\in T} c(u,v)$, considering only "forward" edges
#### Properties of Cuts
##### Lemma
- Let $f$ be a flow in flow network $G$ with source $s$ and sink $t$, and let $(S,T)$ be any cut of $G$.
- Then the net flow across $(S,T)$ is $f(S,T)=|f|$
##### Corollary
- The value of any flow $f$ in a flow network $G$ is bounded from above by the capacity of any cut of $G$
##### Proof of Corollary
- Let $(S,T)$ be any cut of $G$ and let $f$ be any flow. By Lemma and the capacity constraint
$$|f|=f(S,T)=\sum_{u\in S}\sum_{v\in T} f(u,v)-\sum_{u\in S}\sum_{v\in T} f(v,u)\leq \sum_{u\in S}\sum_{v\in T} f(u,v)\leq\sum_{u\in S}\sum_{v\in T} c(u,v)=c(S,T)$$