# **Reinforcement Learning 2024 Coursework**

## **Description**

This repository contains the coursework for the **Reinforcement Learning 2024** course, focusing on practical applications of RL techniques.

## **Coursework 1: Maze Environment and MDP**

The first coursework focuses on resolving a Maze environment, modeled as a **Markov Decision Process (MDP)**. In this environment:

- **Maze Description**: 
  - The maze consists of black squares representing obstacles and dark-grey squares as absorbing states, which correspond to specific rewards. 
  - Absorbing states are terminal and have no transitions to other states.

- **Objective**: 
  - The task is to implement RL techniques that do not require full knowledge of the environment's dynamics, specifically **Monte-Carlo** and **Temporal-Difference learning** methods.

- **Agent Actions**: 
  - The agent can move north, east, south, or west, with a success probability **p**. 
  - If an action fails, the agent has an equal probability of moving in one of the other three directions.

- **Rewards**: 
  - Every action gives a reward of -1. 
  - The episode ends when the agent reaches an absorbing state or exceeds 500 steps. 
  - Absorbing states provide different rewards, with a particular state giving a reward of 500 and others -50, based on the agent's College ID (CID).

- **Personalization**: 
  - The environment parameters, including the success probability **p**, discount factor **γ**, and specific reward states, are personalized based on the last two digits of the student's CID.
 
## **Coursework 2: Cart-Pole Balancing with DQN**

The second coursework involves training an agent to balance a pole attached to a moving cart using **Deep Q-Network (DQN)**. The objective is to maintain the pole in an upright position for as long as possible.

- **Problem Description**: 
  - The goal is to apply a fixed force to the cart either left or right to keep the pole balanced. The action space is discrete with two actions: apply force left (action 0) or right (action 1).
  
- **Observation State**: 
  - The environment provides a state vector of size 4, which includes the cart position, cart velocity, pole angle, and pole angular velocity.
  - Initial conditions start with the cart near the origin and the pole almost upright.

- **Rewards**: 
  - The agent receives a reward of +1 for each step the pole remains upright. The episode ends if:
    - The pole angle exceeds ±12 degrees (0.2094 radians),
    - The cart moves beyond ±2.4 units from the center,
    - The number of steps exceeds 500.

## **Submission Date**

**Submitted on 25th October 2023**




