---
tags:
  - Math
  - SetTheory
---
## Definition
For any sets $a, b$ let $(a, b) = \{\{a\}, \{a, b\}\}$

## Prove that
$\forall a,b,x,y\; (a, b) = (x, y) \Leftrightarrow x=a, y=b$ 

## Proof
$(a, b) = (x, y) \iff \{\{a\},\{a,b\}\} = \{\{x,\{x,y\}\} \implies \left[\begin{gathered} \{x\}=\{a\}\\ \{x\} = \{a,b\}\end{gathered}\right.$
1. $\{x\} = \{a\}$:
	$\{\{a\},\{a,b\}\} = \{\{x,\{x,y\}\} \iff \{\{a\}, \{a, b\} = \{\{a, \{a, y\}\} \iff \underline{\{b\} = \{y\}}$ 
2. $\{x\} = \{a, b\}$:
	$\{\{a\},\{a,b\}\} = \{\{x,\{x,y\}\} \iff \{\{a\}, \{a,b\}\} = \{\{a,b\},\{\{a,b\}, y\}\} \iff$
	$\iff \{a\} = \{a,b\} \iff \{a\} = \{b\} \iff \{x\} = \{a,b\} = \{a\} = \{b\}$ (more generalized case proven in 1.)
Q.E.D. $\blacksquare$