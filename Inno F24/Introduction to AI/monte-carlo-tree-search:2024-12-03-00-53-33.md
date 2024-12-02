---
id: monte-carlo-tree-search:2024-12-03-00-53-33
aliases:
  - Monte Carlo Tree Search
  - MCTS
tags: []
---
# Monte Carlo Tree Search
In computer science, _Monte Carlo tree search_ is a heuristic search algorithm for some kinds of decision processes, most notably those employed in software that plays board games. In that context MCTS is used to solve the game tree.

## Steps
1. Selection
  - Start from root $R$ and select successive child nodes down to a leaf node $L$. The section below says more about a way of choosing child nodes that lets the game tree expand towards most promising moves
2. Expansion
  - Unless $L$ ends the game with a win/loss for either player, either create one or more child nodes or choose from them node $C$
3. Simulation
  - Play a random playout from node C.
  - Simulation can be called playout or rollout
4. Backpropagation
  - Use the result of the playout to update information in the nodes on the path from $C$ to $R$

## Exploration vs Exploitation (UCT)
- It is recommended to select nodes with the highest value f the next formula called _UCT (Upper Confidence Bound)_ applied to trees
$$
UCB = \frac{w_i}{n_i} + c \sqrt{\frac{\ln N_i}{n_i}}
$$
- $w_i$ - \#wins after $i$-th move for the considered node
- $n_i$ - \#simulations after $i$-th move for the considered node
- $N_i$ - \#simulations after $i$-th move for the parent of the considered node
- $c$ - constant that balances exploitation and exploration, theoretically it is $\sqrt2$, but in practice it is chosen empirically
- $\displaystyle\frac{w_i}{n_i}$ - exploitation
- $\displaystyle\sqrt{\frac{\ln N_i}{n_i}}$ - exploartion
