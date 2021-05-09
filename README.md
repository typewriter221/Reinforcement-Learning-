# Reinforcement-Learning-
My understanding of DRL - Pytorch
1. DGANs in Pytorch using Atari game frames from Open AI Gym
2. CatPole Balancing using CrossEntropy Model-Free, Policy-Based, On-Policy
   1. Play N number of episodes using our current model and environment.
   2. Calculate the total reward for every episode and decide on a reward boundary. Usually, we use some percentile of all rewards, such as 50th or 70th.
   3. Throw away all episodes with a reward below the boundary.
   4. Train on the remaining "elite" episodes using observations as the input and
      issued actions as the desired output.
   5. Repeat from step i until we become satisfied with the result.  
3. FrozenLake using CrossEntropy Model-Free, Policy-Based, On-Policy, Discounted Reward - 
   1. Reward 1 on completion Reward 0 on failing.
   2. Calulation discousted reward of each episode to penalize long episodes.
   3. Keeping better performing episodes forto tackel splling randomnes of the enviornment.
   4. Need more than 10K iterations to provide acceptable results. 
