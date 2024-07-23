---
tags:
  - Math
  - FormalSemantics
  - Programming
  - Logic
---
## Formal Syntax
$\langle$program$\rangle$ ::= $\langle$assignment$\rangle$ 
| $\langle$(program)$\rangle$ 
| $\langle$program$\rangle$; $\langle$program$\rangle$ 
| if $\langle$condition$\rangle$ then $\langle$program$\rangle$ else $\langle$program$\rangle$ 
| while $\langle$condition$\rangle$ do $\langle$program$\rangle$

$\langle$assignment$\rangle$ ::= $\langle$variable$\rangle$ := $\langle$expression$\rangle$

$\langle$condition$\rangle$ ::= $\langle$(in)equality$\rangle$ 
| ($\langle$condition$\rangle$) 
| $\neg$$\langle$condition$\rangle$ 
| $\langle$condition$\rangle$$\land$$\langle$condition$\rangle$
| $\langle$condition$\rangle$$\lor$$\langle$condition$\rangle$
...
## [[Operational Semantics]]
- The translation is defined as follows:
	- $F(\langle\text{assigment}\rangle)=1$
	- $F(\alpha;\beta)=F(\alpha)+F(\beta)$
	- $F(\text{if }\phi\text{ then }\alpha\text{ else }\beta)=\min\set{F(\alpha),F(\beta)}$
	- $F(\text{while }\phi\text{ do }\alpha)=0$
## [[Denotational Semantics]]
- Let us fix [[Natural Numbers Representation|natural numbers]] $\mathbb N$ with constants $0$ and $1$ and binary [[Operation]]s "$+$" and "$\min$"
- Let $[\![\;]\!]$ be the following mapping:
	- $[\![$assignment$]\!]=1$
	- $[\![;]\!] = +$
	- $[\![$if - then - else$]\!]=\min$
	- $[\![$while - do$]\!]=0$
	- $[\![\cdot(\alpha,\beta)]\!]=[\![\cdot]\!]([\![\alpha]\!],[\![\beta]\!])$ $\forall \cdot\in\set{";", "\text{if - then - else}", "\text{while - do}"}$
## [[Axiomatic Semantics]]
- TEL axiomatic semantics is an inference system for assertions of the following form $m\leq \alpha\leq n$ where 
	- $m$ is a number 
	- $\alpha$ is a TEL-sentence
	- $n$ is a number or $\infty$
![[Pasted image 20240615192443.png]]
