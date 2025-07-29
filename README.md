# Project-3-Analysis-of-Optimal-Policy-Learning-in-GridWorld-Using-SARSA-and-Q-Learning

## Overview:
This project examines how two classic reinforcement learning algorithms, **SARSA** (on-policy) and **Q-Learning** (off-policy), learn optimal policies in a simple **5×5 GridWorld** environment with terminal and penalty states.

The assignment focuses on:
- Implementing a GridWorld environment with start, penalty (red), and terminal (black) states.

> **Grid Layout Visualization:**  
>
> (S = Start / Blue, R = Penalty / Red, B = Terminal / Black)
>
> ```
> +---+---+---+---+---+
> | B |   |   |   | B |
> +---+---+---+---+---+
> |   |   |   |   |   |
> +---+---+---+---+---+
> | R | R |   | R | R |
> +---+---+---+---+---+
> |   |   |   |   |   |
> +---+---+---+---+---+
> | S |   |   |   |   |
> +---+---+---+---+---+
> ```

- Learning and comparing policies using:
  - SARSA (ε-greedy)
  - Q-Learning (ε-greedy)
- Visualizing:
  - Agent trajectories under learned policies
  - Total rewards per episode over training

The goal is to analyze differences between on-policy and off-policy learning, the exploration-exploitation trade-off, and convergence behavior.


## Repository Contents:
| File                                                        | Description                                                                      |
|-------------------------------------------------------------|----------------------------------------------------------------------------------|
| `GridWorld_RL_SARSA_Q_Learning.ipynb`                       | Main Colab notebook containing code implementations, results, and visualizations |
| `Report.pdf`                                                | Formal report including detailed plots, tables, and analysis of the methods      |
| `README.md`                                                 | Project overview and instructions (this file)                                    |


## How to Run the Code:

#### Option 1: Run on Google Colab (Recommended)
1. Download the notebook `Optimal Policy Learning in GridWorld Using SARSA and Q-Learning.ipynb` from this repository to your computer.
2. Open your browser and go to: [https://colab.research.google.com](https://colab.research.google.com)
3. Click File > Upload notebook in the Colab menu.
4. Upload the downloaded `.ipynb` file.
5. Once opened, run all cells by clicking Runtime > Run all.

#### Option 2: Run Locally with Python 3 and Jupyter
1. Ensure you have Python 3 and Jupyter Notebook installed.
2. Download `GridWorld_RL_SARSA_Q_Learning.ipynb`.
3. Launch Jupyter Notebook and open the downloaded notebook.
4. Run all cells: Kernel > Restart & Run All.

## Requirements:
The notebook uses the following Python libraries:
- numpy
- pandas
- matplotlib
- random
  
These are typically pre-installed in most Jupyter and Colab environments.

## Results:
- Learned Q-tables for both SARSA and Q-Learning.
- Plots of agent trajectories showing the learned path toward terminal states.
- Smoothed plots of total rewards per episode highlighting convergence trends.
- Insights on how SARSA (on-policy) may learn safer routes compared to Q-Learning (off-policy).
