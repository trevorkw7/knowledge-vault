---
created:
  - 2024-05-20 15:32
tags:
  - CSE150B
---

# ❗❓ Information
Related to:: [[Search Problems]]
Tags:: 

# 🌌 Course -> [[CSE 150B]]
---

# ❗ Overal Idea
- Monto Carlo Tree Search!
- For all rounds, we always start with the root node**, try the options at the root node at least once**
- From that node, **unroll a trajectory of the game**, randomly take actions for the two players. 
- Since there is a terminal node, either the max or min will win, this is the end of our sample.
- For the node where the unroll started, we keep track of
	- Number of visits = number of trajectories that are unrolled from this node
	- Number of wins for max player
- After sampling once from each node from the root node, we choose the node that has the highest win rate.![[Screenshot 2024-05-20 at 3.41.45 PM 1.png]] ![[Pasted image 20240520154521.png]]

## ❗ Should we continue to explore this subtree or nah? 
- We use the UCB formula (Upper Confidence Bound) 
- UCB = estimated mean reward + exploration bonus


## Epsilon-Greedy Strategy
- Used to choose whether we want to explore or not
- A higher $\epsilon$ is results in more exploration, playing the other option to increase the sample size of the mean
- For any round $t$:
	- Compare the average reward $\mu_{1}$ and $\mu_{2}$
	- With probability $1-\epsilon$, play the one with better empirical mean
	- With $\epsilon$, play the other one
- **Important**: This $\epsilon$ is a parameter that controls the trade off between and exploitation, this is NOT the same as the $\epsilon$ used in the concentration bound. 
## Concentration Bound
- We use concentration bounds to balance exploration vs exploitation. If the confidence interval is narrow, the algorithm will exploit the estimated best action with higher confidence. If the confidence interval is too wide, the algorithm should continue to explore to reduce uncertainty
- Idea: as I draw more samples / play more rounds, the averages are going to become more reliable
- Concentration bound: $P(|X - \mu > \epsilon) \leq 2e^{-2N\epsilon^2}$
	-  We have an true mean $\mu$ and with confidence $2e^{-2N\epsilon^2}$ we know that sample mean $X$ is in the bounds $[\mu - \epsilon, \mu + \epsilon]$ given we have done $N$ samples/observations
	- $\epsilon$ is our confidence radius: $\epsilon = \sqrt{ \frac{c \log{T}}{N} }$
	-  We are given a decision on whether to play one or another path by using: $\mu_{1} + e_{1} + e_{1} \geq X_{1} + \epsilon_{1} \geq X_{2} + \epsilon_{2} \geq \mu_{2} - \epsilon_{2} +\epsilon_{2}$
	- Our upper confidence bound is: $X_{1} + \epsilon$, the best we can do with high probability
	- Thus substituting $X_{1}$ with our upper confidence bound we get: $\mu_{1} + 2\epsilon_{1} \geq \mu_{2}$
- Results in exponentially less bad plays


## Written Synthesis
