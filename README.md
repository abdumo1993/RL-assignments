# Multi-Armed Bandit Algorithms: E-Greedy, UCB, and Thompson Sampling

## Overview

The **multi-armed bandit (MAB)** problem is a classic scenario in reinforcement learning where an agent must choose between multiple options ("arms") with uncertain rewards, aiming to maximize its total reward over time. The challenge lies in balancing exploration (trying new arms to discover their rewards) and exploitation (choosing the best-known arm).

This project contains a Jupyter Notebook that implements and analyzes three popular algorithms for solving the MAB problem:

- **Epsilon-Greedy**: Selects the best-known arm most of the time (exploitation), but with a small probability (epsilon), it chooses a random arm (exploration). This helps the agent discover potentially better arms while still leveraging current knowledge.

- **Upper Confidence Bound (UCB)**: Chooses arms based on both their average observed reward and the uncertainty (confidence bound) around that estimate. Arms with less data are given a higher chance to be selected, encouraging exploration of less-tried options while still favoring arms with high observed rewards.

- **Thompson Sampling**: Uses a Bayesian approach, maintaining a probability distribution for the reward of each arm. At each step, it samples from these distributions to decide which arm to pull, naturally balancing exploration and exploitation by favoring arms that are likely to be optimal, but still occasionally trying less-certain arms.