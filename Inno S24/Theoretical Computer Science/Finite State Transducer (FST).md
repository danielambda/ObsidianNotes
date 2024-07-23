---
tags:
  - Math
  - TCS
---
## Formal Definition
- A FST is  tuple $T=<Q, I, \delta, q_0, F, O, \eta>$
	- Mostly same as [[Finite State Automaton (FSA)]]
	- $O$ - output [[Alphabet in TCS|alphabet]]
	- $\eta: Q\times I\to O^*$
### Translating a string
- As we did for $\delta$ ([[Finite State Automaton (FSA)]]), we define $\eta^*$ inductively
	- $\eta^*(q,\varepsilon)=\varepsilon$
	- $\eta^*(q,y.i)=\eta^*(q,y).\eta(\delta^*(q,y),i)$
- Remark $\eta^*: Q\times I^*\to O^*$
- $\forall x : \tau(x)=\eta^*(q_0,x)\iff \delta^*(q_0,x)\in F$ 