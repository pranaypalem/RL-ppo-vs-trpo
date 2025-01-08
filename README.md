
# Reinforcement Learning Project

This repository contains the implementation of a Reinforcement Learning (RL) project utilizing OpenAI Gym environments, various RL algorithms, and hyperparameter tuning. The work is organized into structured notebooks and includes both original and tuned models, with supporting files for visualization and evaluation.

---

## Table of Contents

- [Introduction](#introduction)
- [OpenAI Gym](#openai-gym)
- [Reinforcement Learning Models](#reinforcement-learning-models)
- [Hyperparameter Tuning](#hyperparameter-tuning)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Acknowledgements](#acknowledgements)

---

## Introduction

The project explores reinforcement learning strategies applied to environments provided by OpenAI Gym. We implement and evaluate multiple algorithms to understand their behavior in solving predefined tasks. The repository emphasizes hyperparameter tuning and comparative performance analysis.

---

## OpenAI Gym

OpenAI Gym provides the simulation environments used in this project. It enables us to train and evaluate RL agents in a variety of settings, ranging from simple control tasks to complex games. Environments are initialized and interacted with using Gym's API, ensuring robust agent-environment interactions.

---

## Reinforcement Learning Models

### Algorithms
We focus on two key reinforcement learning algorithms:
1. **Proximal Policy Optimization (PPO):**
   - A policy-gradient-based approach for improving agent learning through clipped objective functions.
2. **Trust Region Policy Optimization (TRPO):**
   - A stable policy optimization algorithm using trust regions for policy updates.

### Features
- Both algorithms are implemented with support for tuning hyperparameters.
- Models are saved after training to allow reuse without retraining.

---

## Hyperparameter Tuning

### Parameters Tuned
The project includes extensive tuning of hyperparameters to enhance model performance. Parameters tuned include:
- **Learning Rate:** Controls the step size during optimization.
- **Discount Factor (Gamma):** Defines the weight of future rewards.
- **Policy Network Architecture:** Adjustments in layer sizes and activations.
- **Number of Steps:** Defines the length of each rollout.
- **Seed Values:** Ensures reproducibility of experiments.

### Seed Exploration
Different seeds (e.g., `42`, `123`, `999`, `2024`) are used for random number generation to analyze their impact on model training and performance.

---

## Project Structure

The repository is structured as follows:

```
RL/
├── Original/               # Initial experiments with PPO and TRPO
│   ├── RL_Project-long.ipynb      # Primary notebook with original implementation
│   ├── Models/                    # Saved model weights
│   ├── outputData.pkl             # Raw data from experiments
│   └── results.pkl                # Processed results for visualization
├── Tuned/                  # Hyperparameter-tuned versions
│   ├── RL_Project_Hyper_Final.ipynb  # Final implementation with tuned parameters
│   ├── Models/                      # Saved tuned model weights
│   └── DataVisualize_Final_Hyper.ipynb # Visualization of results
├── videos/                 # Rendered simulation videos
│   └── rl-video-episode-0.mp4
```

---

## Usage

### Prerequisites
- Python 3.x
- Libraries: OpenAI Gym, Stable-Baselines3, NumPy, Matplotlib, Pandas, Pickle

### Running the Code
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd RL
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open and run notebooks:
   - For original experiments: `Original/RL_Project-long.ipynb`
   - For tuned models: `Tuned/RL_Project_Hyper_Final.ipynb`

---

## Acknowledgements

- OpenAI Gym for providing the RL environment.
- [Stable-Baselines3](https://stable-baselines3.readthedocs.io/en/master/) for implementation of RL algorithms.
- All contributors and researchers in reinforcement learning.

---

Feel free to modify this `README.md` file further based on specific details or goals of the project!
