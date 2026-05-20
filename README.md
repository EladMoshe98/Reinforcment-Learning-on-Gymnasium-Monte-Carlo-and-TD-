# Reinforcement Learning – Monte Carlo & TD(0) on Gymnasium

Implementation of **Monte Carlo** and **Temporal Difference (TD(0))** reinforcement learning algorithms across multiple [Gymnasium](https://gymnasium.farama.org/) environments, as part of my CS Master's at IE Business School.

## Algorithms Implemented

- **Monte Carlo (first-visit)** – episodic policy evaluation and control
- **TD(0)** – bootstrapped online value estimation
- **ε-greedy exploration** with decay schedule

## Environments

| Environment | Description |
|-------------|-------------|
| Taxi-v3 | Pick up and drop off passengers on a grid |
| FrozenLake-v1 | Navigate a slippery frozen lake to a goal |
| CliffWalking-v0 | Shortest path avoiding a cliff edge |
| VolcanoWorld (custom) | Custom environment with lava hazards |

## Results

Both algorithms converge on all environments. TD(0) converges faster on stochastic environments; Monte Carlo shows lower variance on episodic tasks with clear terminal states.

## Running

```bash
pip install gymnasium numpy matplotlib jupyter
jupyter notebook rl_assignment.ipynb
```
