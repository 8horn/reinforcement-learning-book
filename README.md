# Reinforcement Learning: An Introduction

Following along Sutton and Barto's book Reinforcement Learning: An Introduction

Please forgive the dirty and unorganized code - I mostly use it this repo to learn and experiment with algorithms introduced in the book. Hopefully, I can refactor most of the code used into a single package once I'm done with the book. 

# Detailed list of progress

Here's a detailed list of completed exercises and implemented methods, ordered by their book appearances.

### Chapter 2: Multi-Armed Bandits ([Notebook](https://github.com/8horn/reinforcement-learning-book/blob/master/Multi-Armed-Bandits.ipynb))


- Full implementation of *K-armed bandit* simulation environment;
- *Epsilon-greedy policy* which balances exploration vs exploitation;
- *Incremental-Implementation* and *Sample-Average Method* which quickly calculates and updates expected value of each possible action;
- *Exponential Recency-Weighted Average* which puts less weights on rewards received long time ago;
- *Optimistic Initialization* which helps enforce exploration in the early steps;
- *Upper Confidence Bounds* (UCB) which selects non-optimal actions in a more clever-fashion by weightening the choice according to potential of the non-optimal action;
- *Gradient Bandit* which learns optimal actions not in terms of rewards, but in terms of preference, comparing the received reward to the average of total rewards received and updating the preferences for all available actions accordingly.

### Chapter 4: Dynamic Programming ([Notebook](https://github.com/8horn/reinforcement-learning-book/blob/master/Dynamic-Programming.ipynb))

- Full implementation of *GridWorld* simulation environment;
- *Iterative Policy Evaluation* which calculates the expected return from any potential state;
- *Policy Iteration* which interleaves iterative policy evaluation with iteraive policy improvement and changes the policy based on newly calculated value function, that depends on that policy.
- *Value Iteration* which produces optimal value function and optimal policy with just a single sweeps along value function.
- Full implementation of *Gamblers Problem* together with value iteration to solve the problem and charts for different probabilities of rolling heads.
- Notes on *Asynchronous Dynamic Programmin* and *Generalized Policy Iteration*
