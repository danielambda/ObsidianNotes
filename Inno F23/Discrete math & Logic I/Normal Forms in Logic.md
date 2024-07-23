___
Tags:
#Math #Logic 
___
## Definitions
- A *literal* is either a variable (positive), or its negation (negative)

|   Literals    |      Not!       |
|:-------------:|:---------------:|
|   $\neg x$    |   $a \lor b$    |
|      $y$      | $\neg (a \& b)$ |
| $\neg \omega$ |  $\neg \neg c$  |

- A *conjunct* (conjunctive term) is a conjunction of literals

|        Conjuncts         |             Not!              |
|:------------------------:|:-----------------------------:|
| $x_1 \& \neg x_2 \& x_3$ | $(a \& \neg b) \lor (a \& c)$ |
|      $\neg a \& b$       |    $\neg a \& (b \lor c)$     |
|           $a$            |          $x \lor y$           |

- A disjunct (disjunctive term) is a disjunctive of literals

|       Conjuncts        |          Not!           |
|:----------------------:|:-----------------------:|
|       $a \lor b$       |     $a \lor c \& b$     |
| $\neg x \lor y \lor z$ | $\neg(a \lor b) \lor c$ |
|          $d$           |        $a \& b$         |

- A [[Disjunctive Normal Form (DNF)]] is a disjunction of conjuncts
- A [[Conjunctive Normal Form (CNF)]] is a conjunction of disjuncts