---
tags:
  - TCS
---
## Definition
- Kleene star*  is a [[Unary relations|unary]] operation either on sets of strings or on sets of symbols or characters
- Given a set $V$, define:
	- $V^0=\{\varepsilon\}$
	- $V^1=V$
	- $V^{i+1}=\{wv:w\in V^i\;\&\;v\in V\}$
	- $\$