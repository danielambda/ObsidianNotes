---
tags:
  - Math
  - Logic
---

is a conjunction of disjuncts

## Algorithm to obtain from the truth table:
- selecting all rows that evaluate to 0
- for each such row, construct a disjunct of literals in the following way:
	- positive literals for corresponding 0 values for the propositional variable
	- negative literals, otherwise (for corresponding 1 value)
- the CNF is the conjunctions of all these disjuncts

## Examples:
CNF for the truth table $T(a, b) = 1000$: $$(a \lor \neg b) \& (\neg a \lor b) \& (\neg a \lor \neg b)$$
$T(x, y) = (1001)$: $$(x \lor \neg y) \;\&\; (\neg x \lor y)$$
$T(x_1, x_2) = (0100)$:$$(x_1\lor x_2)\;\&\;(\neg x_1 \lor x_2)\;\&\;(\neg x_1 \lor \neg x_2)$$
$T(a, b, c) = (01010110)$: $$(a \lor b \lor c)\;\&\;(a \lor \neg b \lor c)\;\&\;(\neg a \lor b \lor c)\;\&\;(\neg a \lor \neg b \lor \neg c)$$
$T(y_1, y_2, y_3) = (10000111)$: $$(y_1 \lor y_2 \lor \neg y_3)\;\&\;(y1 \lor \neg y_2 \lor y_3)\;\&\;(y_1 \lor \neg y_2 \lor \neg y_3)\;\&\;(\neg y_1 \lor y_2 \lor y_3)$$
$T(a, b) = (0110)$, xor operation: $$(a \lor \neg b)\;\&\;(\neg a \lor b)$$ 