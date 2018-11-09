# Personal Work Files for Udacity's Deep Reinforcement Learning Nanodegree Program


## Exercices
+ - [x] **01. Dynamic Programming**
+ - [x] **02. Monte Carlo Control** 
+ - [x] **03. Temporal Difference Control**
+ - [x] **04. Discretization**
+ - [x] **05. Tile Coding**
+ - [x] **06. Deep Q-Networks**
+ - [ ] **07. Robotics**
+ - [x] **08. Hill Climbing**
+ - [x] **09. Cross Entropy**
+ - [x] **10. REINFORCE**
+ - [ ] **11. Proximal Policy Optimization (PPO)**
+ - [ ] **12. Deep Deterministic Policy Gradients (DDPG)**
+ - [ ] **13. Multi-Agent DDPG**
+ - [ ] **14. AlphaZero**


## Labs and Graded Projects
+ - [ ] **P0. Taxi** - general RL.
+ - [x] **P1. Navigation** - value-based methods.
+ - [ ] **P2. Continuous Control** - policy-based methods.
+ - [ ] **P3. Collaboration and Competition** - multi-agent RL.

## Setup
TODO: Dockerfiles for CPU/GPU machines.

```bash
# Environment
conda create --name drlnd python=3.6
source activate drlnd

# OpenAI gym
git clone https://github.com/openai/gym.git
cd gym
pip install -e '.[classic_control]'
pip install -e '.[box2d]'

# Other Dependencies
git clone https://github.com/udacity/deep-reinforcement-learning.git
cd deep-reinforcement-learning/python
pip install .

# Kernel
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```