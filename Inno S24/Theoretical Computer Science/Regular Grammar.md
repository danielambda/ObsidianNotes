---
tags:
  - Math
  - TCS
---
## Definition (Right regular)
- A right regular grammar is a formal [[Generative Grammar|grammar]] $<V_N,V_T,P,S>$ such that all the production rules in $P$ are of one of the following forms:
	- $A\to b, A\in V_N, b\in V_T$
	- $A\to bB, A,B\in V_N, b\in V_T\cup\set\varepsilon$
	- $A\to\varepsilon, A\in V_N$
## Definition (Left regular)
- A right regular grammar is a formal [[Generative Grammar|grammar]] $<V_N,V_T,P,S>$ such that all the production rules in $P$ are of one of the following forms:
	- $A\to b, A\in V_N, b\in V_T$
	- $A\to Bb, A,B\in V_N, b\in V_T\cup\set\varepsilon$
	- $A\to\varepsilon, A\in V_N$
## Fact
- In [[Chomsky Hierarchy]] type 3
Right regular = Left regular = [[Regular Language]] = [[Finite State Automaton (FSA)]]