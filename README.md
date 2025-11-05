**RL Navigation Agent (Q-Learning)**

A simple Reinforcement Learning (RL) project where an agent learns to navigate a 2D grid maze from start to goal while avoiding obstacles.
The project demonstrates the fundamentals of Q-Learning, a core algorithm in reinforcement learning and robotics navigation.

**Project Overview**

This project simulates an autonomous navigation task using a custom GridWorld environment built with Python and Gymnasium.
An agent starts at a defined location and learns through trial and error how to reach the goal efficiently, using only feedback (rewards) from the environment.

**Learning Approach**

The agent is trained using Q-Learning, a model-free reinforcement learning algorithm.
It learns an optimal policy (state → action) by maximizing expected future rewards.

**Key Concepts:**

Exploration vs Exploitation using ε-greedy policy
Reward shaping to encourage shorter, safer paths
State-value updates with Bellman Equation

**Environment Setup**
Symbol	Meaning
S	Start position
G	Goal position
#	Obstacle
.	Free path
A	Agent position

**Example Maze:**

S . . . . .
# # . # # .
. . . . # .
. # # . . .
. . . # # .
. . . . . G

**Model Details**
Parameter	Value
Learning Rate (α)	0.7
Discount Factor (γ)	0.95
Exploration Rate (ε)	Decayed from 1.0 → 0.05
Episodes	2000
Algorithm	Q-Learning (Tabular)

**Results**

The agent learns to reach the goal efficiently after several hundred episodes.
Reward curve shows convergence over time.
Final learned path is visualized directly in the console.
Metric	Description
  Navigation	Agent successfully finds optimal path
  Loss	Implicitly minimized through Q-value updates
  Goal	100% reach rate after convergence
