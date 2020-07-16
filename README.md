## Gridworld with Monte Carlo on-policy first-visit MC control (for ε-greedy policies)

### Overview

This is my implementation of an on-policy first-visit MC control for epsilon-greedy policies, which is taken from page 1 of the book *Reinforcement Learning* by *Richard S. Sutton and Andrew G. Barto*

The algorithm in the book is as follows:

![Algorithm](img/algo.png?raw=true "MC Algorithm")

### Hyperparameters

**ε** = 0.1

**γ** = 1

### Convergence

Things start to converge around the 500th episode; and by episode 5000 the policy is in an optimal state. By the 50,000th episode the Q-values have stabilized to about 1 decimal place:

![Convergence](img/gridworld.png?raw=true "Convergence")

### Q-States

In the following Q-state table you can see some of the final Q-states in addition to how many times each Q state was refresh: as you can see, the optimal Q-states are visited most of the time; however, there is some exploration happening thanks to the ε-greedy policy.

![QStates](img/qstates.png?raw=true "Q-States")
