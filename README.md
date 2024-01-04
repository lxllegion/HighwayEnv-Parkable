# Safe-ParkDRL for School Zones

Human-to-car interaction for autonomous parking is a research area that has received significantly less attention than car-to-car interactions. However, preventing harm to people is equally, if not more, important than avoiding col- lisions with other vehicles or structures. To address this is- sue, we introduce our Soft Actor-Critic (SAC) model, which is a modification of Stable Baselines 3. Our model detects both human-to-car and car-to-car interactions and safely parks the car in the Highway.env simulation. Through this work, we aim to contribute to safe autonomous parking tasks.

[FULL PDF](https://github.com/lxllegion/Safe-ParkDRL/blob/master/final_Parkable.pdf)


## Installation

First, install highway-env
`pip install highway-env`

Then, use this page to add more Objects

## Usage

```python
import gymnasium as gym

env = gym.make('highway-v0', render_mode='human')

obs, info = env.reset()
done = truncated = False
while not (done or truncated):
    action = ... # Your agent code here
    obs, reward, done, truncated, info = env.step(action)
```

## Documentation

Read the [documentation online](https://farama-foundation.github.io/HighwayEnv/).

## Citing

If you use the project in your work, please consider citing it with:
```bibtex
@misc{Safe-ParkDRL,
  author = {Andy Seoho Yun, Xinlei Liu, Chanseok Oh},
  title = {Safe-ParkDRL for School Zones},
  year = {2023},
  journal = {GitHub repository}
}
```
