---
tags:
  - Math
  - TCS
---
## Definition
- A configuration (or a snapshot) $c$ of a [[Turing Machine]] with $k$ tapes is the following $(k+2)$ tuple: $$c=<q,x\uparrow y,\alpha_1\uparrow \beta_1,\dots,\alpha_k\uparrow \beta_k>$$
- Where 
	- $q\in Q$
	- $x\in(\Sigma\cup\set\_)^*, y=y'\cdot\_, y'\in\Sigma^*$
	- $\alpha_i\in(\Gamma\cup\set\_)^*, \beta_i=\beta'_i\cdot\_,\beta'\in\Gamma^*, 1\leq i\leq k$
	- $\uparrow\not\in\Sigma\cup\Gamma$ is the tape head symbol