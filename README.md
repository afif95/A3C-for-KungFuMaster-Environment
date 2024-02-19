# A3C for Kung Fu in OpenAI Gym

This repository contains code for training an A3C agent to play Kung Fu MasterDeterministic-v0 environment in OpenAI Gym.

### Key Features:

- Implementation of the A3C (Asynchronous Advantage Actor-Critic) algorithm for multi-agent training.
- Preprocessing pipeline for Kung Fu observations using the PreprocessAtari wrapper.
- Environment batching for parallel interaction with multiple environments.
- Evaluation of the trained agent on single episodes.
- Video recording and visualization of the agent's gameplay.
- Train the agent for 3000 episodes and periodically show the average agent reward during training.

  **Environment:** https://gymnasium.farama.org/environments/atari/kung_fu_master/

  
![a](https://github.com/afif95/A3C-for-KungFuMaster-Environment/assets/34897455/f86488d1-6b0a-4ed3-b810-10b518389122)


https://github.com/afif95/A3C-for-KungFuMaster-Environment/assets/34897455/b55dfe56-226b-4cba-b325-352cd14fcd4c


### Requirements:

Python 3
PyTorch
NumPy
OpenAI Gym
tqdm

### Additional Notes:

The script currently trains 10 agents in 10 parallel environments. You can modify these numbers in the number_environments and EnvBatch class.
The reward scaling (batch_rewards *= 0.01) is optional and might need adjustment depending on your environment and training dynamics.
