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