---
tags:
  - Math
  - TCS
---
## Definition
- A grammar is a tuple $<V_N, V_T, P, S>$ where
	- $V_n$ is the nonterminal [[Alphabet in TCS|alphabet]] (or vocabulary)
	- $V_T$ is the terminal [[Alphabet in TCS|alphabet]] (or vocabulary)
	- $V=V_N\cup V_T$
	- $S\in V_N$ is a particular element of $V_N$ called initial symbol
	- $P\subseteq V^* V_N V^*\times V^*$ is the finite set of rewriting rules or **productions**

- A grammar $G=<V_N, V_T, P, S>$ generates a [[Language in TCS|language]] on the [[Alphabet in TCS|alphabet]] $V_T$
## Productions 
- A production is an element of $V^*V_NV^*\times V^*$ 
	- This is usually denoted as 
	- $<\alpha, \beta>$ where 
		- $\alpha \in V^*V_NV^*,\beta \in V^*$
## Example
- $G=<\set{S, A, B, C, D}, \set{a, b, c}, P, S>$
	- $P=\set{S\to aACD, A\to aAC|\varepsilon, B\to b, CD \to BDc, CD \to DC, D\to\varepsilon}$
- Some derivations
	- $S\to a\textbf A CS\to a\textbf{CD}\to a\textbf B D\to ab\textbf D c\to abc$
	- $S\to a\textbf ACS\to aaACCD\to aaCBDc \to aaBCDc\to ...\to aabbcc$
## Classification
#### **General**
- (also called **unrestricted**) grammars are grammars without any limitation on productions
	- They correspond to type 0 in the [[Chomsky Hierarchy]] ([[Turing Machine]])
	- Both context-free grammars and regular grammars are unrestricted
#### **[[Context-Sensitive Grammars|Context-Sensitive]]**
- grammars are [[Chomsky Hierarchy|Type-1]] grammars with rules:
	- $\alpha A\beta\to \alpha\gamma\beta$, where $A$ is a nonterminal and $\alpha, \beta,\gamma$ are strings of terminals and non-terminals, $|\gamma| >0$
#### **[[Context-Free Grammar|Context-Free]]**
- grammars (CFG):
	- foreach $\alpha\to\beta\in P: |\alpha|=1\;\&\;\beta \in V=V_N\cup V_T$
	- They are called context-free because the rewriting of $\alpha$ does not depend on its context
	- CFGs are the same as the [[Backus-Naur Form (BNF)]]s used for defining the syntax of programming languages
		- They are well fit to define typical features of programming and natural languages
		- Regular grammars are also context-free grammars
		- But not vice-versa
#### Right-Linear 
- All productions have form:
	- $A\to xB$
	- or $A\to x$
	- x is a string of terminals
#### Left-Linear
- All productions have form:
	- $A\to Bx$
	- or $A\to x$
	- $x$ is a string of terminals
#### [[Regular Grammar]] 
- [[Chomsky Hierarchy|Type-3]] grammars restrict productions to 
	- a single nonterminal on the left-hand side
	- right-hand side consisting of 
		- a string of terminals
		- possible followed by a single non-terminal
		- or preceded, but **not both** in the same grammar