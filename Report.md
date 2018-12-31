## Context

The challenge of this project is to teach an agent to perform a challenge in a game of collecting as many yellow bananas as possible. A reward of `+1` is provided for collecting a yellow banana, and a reward of `-1` is provided for collecting a blue banana. 

The program was developed in Deep Q-learning, based on the course code (Deep_Q_Network_Solution.ipynd). 

In the project folder is the Unity environment (Banana.app), the Jupyter file to run and two files with the DQN code and the model.

### DQN Hyper Parameters  

- n_episodes (int): maximum number of training episodes: 2000
- max_t (int): maximum number of timesteps per episode: 10000
- eps_start (float): starting value of epsilon, for epsilon-greedy action selection 1.0
- eps_end (float): minimum value of epsilon: 0.01
- eps_decay (float): multiplicative factor (per episode) for decreasing epsilon: 0.99


### DQN Agent Hyper Parameters

- BUFFER_SIZE (int): replay buffer size: int(1e5)
- BATCH_SIZE (int): mini batch size: 128
- GAMMA (float): discount factor: 0.99
- TAU (float): for soft update of target parameters: 1e-3
- LR (float): learning rate for optimizer: 5e-4 
- UPDATE_EVERY (int): how often to update the network: 3


## Performance and  Plot of Rewards

https://github.com/rubenbet/udacitybanana/blob/master/Results.png

Episode 100 Average Score: 1.30
Episode 200 Average Score: 6.01
Episode 300 Average Score: 9.16
Episode 400 Average Score: 11.38
Episode 436 Average Score: 13.03
Environment solved in 436 episodes! Average Score: 13.03

## Improvements

In the future, different DQN algorithms could be combined and tested Prioritized DDQN and Dueling DDQN both use double Q-learning, and Dueling DDQN was also combined with prioritized experience replay (https://arxiv.org/pdf/1710.02298.pdf).



