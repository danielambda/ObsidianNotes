---
tags:
  - Math
  - TCS
---
## Definition
- A context-sensitive grammar is a formal [[Generative Grammar|grammar]] $<V_N, V_T, P,S>$ such that all the production rules in $P$ are the following forms: $$s_1As_1\to s_1\gamma s_2$$
- where $A\in V_N, s_1, s_2,\gamma\in(V_T\cup V_N)^*\;\&\;\gamma\not=\varepsilon$
## Fact
- Contexct-sensitive grammars = [[Linear-Bounded Automaton]]