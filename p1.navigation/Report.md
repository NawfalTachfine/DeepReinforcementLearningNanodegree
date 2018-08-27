# Project 1 - Navigation
## Training a DeepRL agent to solve the Unity Banana Collector task

### Solution
I started out simple, re-purposing the vanilla Deep Q-Learning Network from the corresponding lesson, with one hidden layer comprised of 64 neurons. To my surprise, it solved the task in **less than 500** episodes! It goes to show how powerful them neural networks are! :smile:

![](scores.png)

There were no changes to the hyper-parameters from the DQN lesson. The network uses a **batch size** of **64** examples and a **learning rate** of **0.0005**. The agent updates the target Q-network **every 4 steps** using a **discount factor** of **0.99**.

---

### Next Steps
This is barely the beginning and there are plenty of things to improve:
+ The first noticeable issue is how unstable is the training, seeing how noisy is the reward plot. I suspect using Double DQN would help.
+ I think the task can be solved faster. I plan to add improvements incrementally to go from vanilla DQN to Rainbow. I am very curious to see how that goes.
+ Lastly, I plan to give solving the associated visual task a try to see if the Google Deepmind ConvNet architecture generalizes to this environment. Intuitively, I think it would take longer to solve the task but I would like to verify that.