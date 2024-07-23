---
tags:
  - Math
  - TCS
---
## Lemma
- If $L\subseteq \Sigma^*$ is a [[Language in TCS|language]] recognized by a [[Pushdown Automaton (PDA)|PDA]] then there exists $m\geq$ such that any $w\in L$ with $|w|\geq m$ can be represented as $w=abcde$ such that
	- $|bd| >0$
	- $|bcd| \leq m$
	- $\forall i \geq0:ab^icd^ie\in L$
## Corollary
- If for any $m\geq 1$ such that there is $w\in L$ such that $|w|\geq m$ and for any representation $w=abcde$ such that $|bd| > 0, |bcd|\geq m$
$$\exists i\geq 0:ab^icd^ie\not\in L$$
then $L\subseteq\Sigma^*$ is __not__ recognized by any [[Pushdown Automaton (PDA)|PDA]] 