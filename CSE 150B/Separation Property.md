---
created:
  - 2024-04-10 00:59
tags:
  - CSE150B
---

# ❗❓ Information
Related to:: [[Dijkstra]]
Tags:: 

# 🌌 Course -> [[CSE 150B]]
---

# ❗ Idea
- Any path that goes from the explored set to the unexplored set has to pass the frontier
- ![[Pasted image 20240410011301.png]]
- Can be used for debugging because visually we can inspect if there is any "leaking" between the unexplored and explored part
- Proof by Induction:
	- In the beginning when we make the frontier the starting node it as this property
	- Then for all base case + 1 steps, we maintain this property 
		- Simple case: all nodes are in the explored case so algorithm knows about it
		- Complicated case: arbitrary paths that go through unexplored node
			- Separation property means that paths that go through unexplored nodes must cross through the frontier at least once.
			- Since priority queue on frontier sorts by cost, $C(goal) \leq C(n)$ for n being the node that this arbitrary path goes through
			- Since along this imaginary path, the cost cannot decrease (Dijkstra requires non-negative costs), then this arbitrary path has higher or equal cost than the path given by the Dijkstra algorithm