---
tags:
  - CompArch
  - Math
a.k.a.: "[[Finite State Automate (FSA)]]"
---
## Definition
- A set if states $S$ (circles), an initial state $s_0$ and a transition function that maps from the current input and current state to output and the next state (arrows between states)
## Mathematical Definition
- Consider
	- $S = s_0, s_1,...,s_{n-1}$ is a finite set of states
	- $I = i_0, i_1, ..., i_{k-1}$ is a finite set of input values
	- $O = o_0, o_1, ..., o_{m-1}$ is a finite set of output values
- Definition
	- A finite state machine is a [[Function]]:
	- $F: (S\times I) \to (S\times O)$
## Formally
- An FSA is a tuple $<Q, A, \delta, q_0, F>$
	- $Q$ is a finite set of states
	- $A$ is the input alphabet
	- $\delta$ is a (partial) transition function:
	- $\delta: Q\times A \to Q$
	- $q_0\in Q$ is an initial state
	- $F\subseteq Q$ is a set of final states
## Representations and Implementations
- Function can be represented with a state transition diagram
- With [[Combinational Logic Circuits]] and [[Registers|registers]], any FSM can be implemented in hardware
## Notes
- State transitions are controlled by the clock 
	- On each clock cycle the machine checks the inputs and generates a new state (could be same) and new output

## Hardware Implementation
![[Pasted image 20231004160226.png]]

## Example
- Simple Cache Controller
![[Pasted image 20231004155031.png]]
