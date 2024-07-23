---
tags:
  - Math
  - TCS
  - Algorithms
---
## This is an
- algorithm to get [[Finite State Automaton (FSA)]] from [[Regular Expression]]
## Algorithm
#### Concatenation
expression $s\cdot t$ is converted to 
![[Pasted image 20240404142700.png]]
$N(s)$ and $N(t)$ are the N[[Finite State Automaton (FSA)|FSA]] of the subexpression $s$ and $t$, respectively.
#### Union 
expression $s|t$ is converted to
![[Pasted image 20240404142944.png]]
$N(s)$ and $N(t)$ are the (N)[[Finite State Automaton (FSA)]] of the subexpression $s$ and $t$, respectively.
#### [[Kleene Star]]
expression $s^*$ is converted to
![[Pasted image 20240404143547.png]]