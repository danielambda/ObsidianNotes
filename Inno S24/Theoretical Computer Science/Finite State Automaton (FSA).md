---
tags:
  - Math
  - TCS
a.k.a.: "[[Finite State Machine]]"
---
## Formal Definition
- An FSA is a tuple $<Q, A, \delta, q_0, F>$ where
	- $Q$ is the set of states
	- $A$ is the [[Alphabet in TCS|alphabet]]
	- $\delta$ is a partial transition [[Function]], given by
		- $\delta: Q\times A\to Q$
	- $q_0\in Q$ is called initial state
	- $F\subseteq Q$ it the set of final sets
### Move [[Sequence]]
- $\delta^*: Q\times A^*\to Q$
- $\delta^*$ is inductively defined from $\delta$
	- $\delta^*(q,\varepsilon)=q$
	- $\delta^*(q,y.i)=\delta(\delta^*(q,y),i)$
- Acceptance:
	- $\forall x: x\in L\iff \delta^*(q_0,x)\in F$
		- $L$ is a [[Language in TCS|language]] 
## Informal Definition
#### States
- An FSA has a finite set of states
	- A system has a limited number of configurations
#### Inputs
- An FSA is defined over an [[Alphabet in TCS|alphabet]]
- The symbols of the [[Alphabet in TCS|alphabet]] represent the input of the system
#### Transition among states
- When in input is received the system changes its state
- The passage between stated is performed through transitions
- Transitions are graphically represented as arrows
