# AI Course Projects

This repository contains my homework and final project for the Introduction to Artificial Intelligence course.

The projects include implementations of search algorithms, planning methods, and other AI techniques learned during the course.


# AI Homework 1 – Heuristic Search AI

This repository contains my solution for **Homework 1 in the Introduction to Artificial Intelligence course**.

   ## Description

   The assignment focuses on solving a **colored blocks tower problem** using search algorithms.
   Given an initial configuration of cubes and a goal configuration of visible colors, the program finds the **optimal sequence of actions** to reach the goal.

   The solution implements the **A* search algorithm** together with heuristic functions to efficiently explore the state space.

   ## Files

   * `heuristics.py` – heuristic functions (base and advanced)
   * `color_blocks_state.py` – representation of the tower state and operators
   * `search.py` – search algorithm implementation
   * `search_node.py` – search node structure

  ## Language

  Python 3.10

# AI Homework 2 – Two player games

This repository contains my solution for Homework 2 in the Introduction to Artificial Intelligence course.

## Description

The assignment focuses on the **IsoKnight two-player game**, where each player moves a knight-like piece on a board with special rules. The goal is to implement AI algorithms that evaluate game states and select optimal moves.

The solution implements **Minimax**, **Alpha-Beta pruning**, and **heuristic evaluation** to efficiently explore the game tree. An optional advanced heuristic can be used for improved performance on larger boards.

## Files

- `heuristics.py` – heuristic functions (base and advanced)  
- `alpha_beta_isoKnight.py` – Minimax with Alpha-Beta pruning  
- `heuristic_alpha_beta_isoKnight.py` – Alpha-Beta with heuristics  
- `minimax_isoKnight.py` – Minimax algorithm  
- `player_agent.py` – player agent logic  
- `game_state.py` – representation of the game state  
- `game_engine.py` – game engine and runner  

## Language

Python 3.x  

# AI Homework 3 – Planning

This repository contains my solution for Homework 3 in the Introduction to Artificial Intelligence course.

## Description

The assignment focuses on creating a **community garden planning domain** using PDDL. Volunteers in the town of Harmonyville must collect tools, till soil, plant seeds, and water the garden to achieve a thriving garden. The goal is to define the domain, problem files, and actions to allow a **domain-independent planner** to generate valid action sequences.

The solution uses **uni_planner.py** to run the PDDL domain and problem files, producing plans that complete the garden successfully.

## Files

- `community_garden.pddl` – domain definition  
- `community_garden_problem_v1.pddl` … `v5.pddl` – problem instances  
- `community_garden_problem_v1_solution.txt` … `v2_solution.txt` – corresponding solutions  
- `uni_planner.py` – domain-independent planner (provided, do not modify)  

## Requirements

- Python 3.10  
-bash

# AI Main Project – Agentic AI

This repository contains my solution for the main project (Homework 4) in the Introduction to Artificial Intelligence course.

## Description

The project focuses on building an **LLM-based multi-agent system** using LangGraph. The system consists of:

1. **Your implemented agent** – solves one of the previous assignments (search, games, or planning).  
2. **LLM agent** – attempts to solve the same problem independently.  
3. **LLM as a judge** – compares solutions from both agents, explains differences, and evaluates results.

The goal is to observe how an LLM agent performs compared to your implementation and to analyze outputs and heuristics.

## Files

- `AgenticAI.ipynb` – main Jupyter notebook with implementation, agent comparison, and evaluation.

## Requirements

- Python 3.x  
- LangGraph library (for LLM agents)  
- Optional: local LLM models (Gemini, Ollama, IBM Granite) for offline execution

## Usage

Run the notebook to execute both agents, compare solutions, and generate outputs for the selected assignment:

- For **search**, prints solution cost.  
- For **games**, prints board state and heuristic evaluation.  
- For **planning**, prints generated plan.  

Outputs are displayed and saved within the notebook for submission and evaluation.

# AI Homework 5 – Reinforcement Learning & MDP

This repository contains my solution for Homework 5 in the Introduction to Artificial Intelligence course.

## Description

The assignment focuses on implementing **Reinforcement Learning (Q-Learning)** and **Markov Decision Process (Value Iteration)** algorithms for two problems:

1. **Cliff Walking** – The agent learns the optimal path to navigate safely across a cliff environment.  
2. **Gambler’s Problem** – The agent decides how much to bet to reach a goal amount given probabilistic outcomes.

The goal is to compute optimal policies and value functions for these environments using **Q-Learning** and **Value Iteration**, and visualize the results.

## Files

- `q_learning.py` – Q-Learning algorithm implementation  
- `value_iteration.py` – Value Iteration for MDPs  
- `common.py` – shared utilities and environment setup  
- `plotting.py` – functions to visualize results  
- `cliff_walking_experiment.py` – experiment runner for Cliff Walking  
- `gamblers_experiment.py` – experiment runner for Gambler’s Problem  
- `requirements.txt` – dependencies  

## Requirements

- Python 3.10  
- Gymnasium:
```bash
pip install "gymnasium[toy-text]"


