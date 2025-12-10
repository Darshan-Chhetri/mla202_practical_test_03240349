# mla202_practical_test_03240349
this repository contains the solutions for the three problems for mla202 practical test:

Q-learning on GridWorld
The problem involves using Q-learning to train an agent to navigate a 5x5 GridWorld, where the agent must move from a start position (0,0) to a goal (4,4) while avoiding walls. 
Q-learning, a model-free reinforcement learning technique, is used to learn an optimal policy by updating a Q-table through trial and error, where the agent receives rewards based on its actions. 
The agent aims to maximize its cumulative reward by balancing exploration (trying random actions) and exploitation (choosing the best-known action).

Deep Q-Network (DQN) for cartpole
The problem involves training a Deep Q-Network (DQN) to solve the CartPole-v1 task, where the goal is to balance a pole on a cart by taking discrete actions (left or right) based on the environment's state. 
DQN, a reinforcement learning technique, uses a neural network to approximate the Q-value function, guiding the agent's decisions. 
The agent learns from experience using a replay buffer and an epsilon-greedy strategy for balancing exploration and exploitation

Debugging and comparing Q-learning 
The problem involves identifying and fixing bugs in a Q-learning implementation for solving the FrozenLake-v1 environment. 
The issues included incorrect Q-table initialization, improper action selection (minimizing Q-values instead of maximizing), a flawed Q-learning update rule (missing learning rate), 
and no epsilon decay for exploration-exploitation balance.

