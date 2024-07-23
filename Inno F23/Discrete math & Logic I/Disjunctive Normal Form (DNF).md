___
Tags:
#Math #Logic
___
is a disjunction of conjuncts

## Algorithm to obtain from the truth table:
- selecting all rows that evaluate to 1
- for each such row, construct a conjunct of literals in the following way:
	- positive literals for corresponding 1 values for the propositional variable
	- negative literals, otherwise (for corresponding 0 value)
- the DNF is the disjunctions of all these conjuncts

## Examples:
DNF for the truth table $T(a, b) = (0101)$: $$(\neg a \& b) \lor (a \& b)$$
$T(x, y) = (1001)$: $$(\neg x \& \neg y) \lor (x \& y)$$
$T(x_1, x_2) = (0100)$: $$\neg x_1 \& x_2$$
$T(a, b, c) = (01010110)$: $$(\neg a \& \neg b \& c) \lor (\neg a \& b \& c) \lor (a \& \neg b \& c) \lor (a \& b \& \neg c)$$
$T(y_1, y_2, y_3) = (10000111)$: $$(\neg y_1\;\&\;\neg y_2\;\&\;\neg y_3)\lor(y_1\;\&\;\neg y_2\;\&\;y_3)\lor(y_1\;\&\;y_2\;\&\;\neg y_3)\lor(y_1\;\&\;y_2\;\&\;y_3)$$
