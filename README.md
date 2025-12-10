# mla202_practical_test_03240349
this repository contains the solutions for the three problems for mla202 practical test:

**Q-learning on GridWorld:**
The problem involves using Q-learning to train an agent to navigate a 5x5 GridWorld, where the agent must move from a start position (0,0) to a goal (4,4) while avoiding walls. 
Q-learning, a model-free reinforcement learning technique, is used to learn an optimal policy by updating a Q-table through trial and error, where the agent receives rewards based on its actions. 
The agent aims to maximize its cumulative reward by balancing exploration (trying random actions) and exploitation (choosing the best-known action).

**solution overview:**
In this task, Q-learning was applied to a 5x5 GridWorld, where the agent had to navigate from a start (top-left) to the goal (bottom-right) while avoiding walls. The agent could take one of four actions (up, down, left, right) at each step, and the Q-table was updated using the standard Q-learning formula:
Q(s,a)←Q(s,a)+α(r+γ⋅(max⁡)┬a Q(s^',a)-Q(s,a))

Training was done over 1000 episodes with parameters: α=0.1, γ=0.99, and ϵ=0.1.
The learned policy was visualized, showing the best action for each state in the grid. By the end of training, the agent achieved an average reward of 9.03 out of 10 in the final 100 episodes. In testing, the agent successfully reached the goal in 100% of the episodes, averaging 8 steps per goal.
The Q-table had 80 non-zero values, with a maximum Q-value of 10.00, indicating efficient learning and navigation.


**Deep Q-Network (DQN) for cartpole:**
The problem involves training a Deep Q-Network (DQN) to solve the CartPole-v1 task, where the goal is to balance a pole on a cart by taking discrete actions (left or right) based on the environment's state. 
DQN, a reinforcement learning technique, uses a neural network to approximate the Q-value function, guiding the agent's decisions. 
The agent learns from experience using a replay buffer and an epsilon-greedy strategy for balancing exploration and exploitation

**solution overview:**
The solution implements a Deep Q-Network (DQN) to solve the CartPole-v1 environment. The DQN consists of a neural network with two hidden layers, each with 128 units, to approximate the Q-function. The agent uses an epsilon-greedy strategy, initially exploring and then exploiting the learned Q-values. Experience replay is used to store and sample transitions, stabilizing training. A target network is periodically updated to stabilize Q-value predictions. The agent is trained over 500 episodes, with training stopping when the average reward over the last 100 episodes exceeds 475. After training, the agent is tested for 10 episodes, and its performance is evaluated. The approach demonstrates how DQN effectively learns to solve CartPole-v1 using reinforcement learning.

**Debugging and comparing Q-learning:**
The problem involves identifying and fixing bugs in a Q-learning implementation for solving the FrozenLake-v1 environment. 
The issues included incorrect Q-table initialization, improper action selection (minimizing Q-values instead of maximizing), a flawed Q-learning update rule (missing learning rate), 
and no epsilon decay for exploration-exploitation balance.

