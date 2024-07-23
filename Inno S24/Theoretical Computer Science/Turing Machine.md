---
tags:
  - Math
  - TCS
---
## Definition (1 tape)
- A Turing Machine with 1 tape is a tuple $T=<Q, \Sigma, \Gamma, \delta, q_0, Z_0, F>$
- Where
	- $Q$ is a finite set of states
	- $\Sigma$ is the input [[Alphabet in TCS]]
	- $\Gamma$ is the memory [[Alphabet in TCS]]
	- $\delta: (Q-F)\times(\Sigma\cup\set{\_})\times(\Gamma\cup\set{\_})\to Q\times(\Gamma\cup\set\_)\times\set{R,L,S}^2$ is the transition [[Function]]
	- $q_0\in Q$ is the initial state
	- $Z_0\in\Gamma$ is the initial memory symbol
	- $F\subseteq Q$ is the set of final states
## Definition ($k$ tapes)
- A Turing Machine with $k$ tapes is the same tuple but
	$$\delta:(Q-F)\times(\Sigma\cup\set\_)\times(\Gamma\cup\set\_)^k\to Q\times(\Gamma\cup\set\_)^k\times\set{R,L,S}^{k+1$}$$
## Special symbols:
- $R$: move the head one position the right
- $L$: move the head one position to the left
- $S$: stand still
-  $\_:\_\not\in\Gamma\cup\Sigma$ is a special blank symbol on the tapes
## Remarks 
- The transition [[Function]] $\delta$ can be partial
- No transition outgoing from the final states
## [[Turing Machine Configuration]]
## Turing Thesis
- A [[Function]] on the [[Natural Numbers Representation|natural numbers]] can be calculated by an effective method if and only if it is computable by a *Turing machine*
## Example
![[Pasted image 20240321125721.png]]
