# Project 3 - Collaboration and Competition
## Training multiple DeepRL agents to solve the Unity Tennis task

### Solution
This solution is based on the MADDPG algorithm, using seperate actors and critics for each agents and a shared memory buffer. The code base is adapted from my previous project, which was itself based on the DDPG-Pendulum exercise. The `Group` class, which is in charge of handling the multiple agents, is not restricted to the case of dueling single agents and should work for more that 2 without any changes.

The agents solved the task after **2860** episodes. I kept the same set of hyperparameters from the previous project: both actor and critic networks have 2 fully-connected hidden layers of **128** nodes, both trained with a learning rate of **0.001**, using mini-batches of **256**, a replay buffer of **100000**, and a discount of **0.9**. The Ornstein-Uhlenbeck noise has a sigma of **0.1** and the soft update is made using a tau of **0.001**.

The scores are quite noisy, as it is often the case with multi-agent tasks, but they did not crash as I kept the agents for 10000 episodes total. 

![](scores.png)

---

### Next Steps
The is the first solution I tried my hands on. Here are so
+ Experiment further with hyperparameters to solve the task faster.
+ Compare performance with that of other MADDPG variants: shared actors, shared critics, shared actors *and* critics.
+ Stabilization techniques
+ Evaluate the same solution on the Soccer task.