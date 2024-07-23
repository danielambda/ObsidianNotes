---
tags:
  - Math
  - TCS
---
## Indeed 
- PDA is just a [[Finite State Automaton (FSA)|FSA]] with (destructive) external memory. Also, [[Stack]] has to be mentioned here
![[Pasted image 20240229134040.png]]
 - PDAs differ from [[Finite State Automaton (FSA)|FSAs]] in two ways:
	 1. They can use the top of the [[Stack]] to decide which transition has to be made
	 2. They can manipulate the [[Stack]] as a part of performing a transition
## Formally
- A PDA is a tuple $<Q, I, \Gamma, \delta, q_0, Z_0, F>$
	- $Q$ is a finite set of states
	- $I$ is the input [[Alphabet in TCS|alphabet]]
	- $\Gamma$ is the [[Stack]] [[Alphabet in TCS|alphabet]]
	- $\delta$ is the transition [[Function]]
	- $q_0\in Q$ is the initial state
	- $Z_0\in \Gamma$ is initial [[Stack]] symbol
	- $F\subseteq Q$ is the set of final states
#### Transition [[Function]]
- $\delta$ the transition [[Function]]
- $\delta: Q\times(I\cup \set{\varepsilon})\times\Gamma\to Q\times \Gamma^*$
- $\delta(q,i,A)=<p,\alpha>$
- Graphical notation
![[Pasted image 20240229150426.png]]
## Remarks
- $Q, I, q_0, F$ are defined as in [[Finite State Automaton (FSA)]]
- $\delta$ is a partial [[Function]] 
- $Z_0$ is not essential, it is just useful to simplify definitions
- $\delta(q,\varepsilon,A)=<p,\alpha>$
	- An "$\varepsilon$ move" is a spontaneous move
	- It does not mean that input is empty!
	- It means that move happens immediately witout consuming the input
## Conventions
- The [[Stack]] grows bottom-up
- The input strings are read left to right
- The other way around is possible, but is important to be coherent
## Moves of PDA
- Depending on
	- The symbol read from the input (but in could also read nothing)
	- The symbol read from the top of the [[Stack]]
	- The state of the control device
- The PDA
	- Changes its state
	- Moves ahead the scanning head of the input
	- Changes the symbol read from the [[Stack]] with a string $\alpha$ (possibly empty)
## From week 11
- PDA without $\varepsilon$-moves are also knows as **realtime dererministic PDA**
- They are less powerful than DPDA