---
created:
  - 2024-05-22 18:04
tags:
  - CSE150B
---

# ❗❓ Information
Related to:: 
Tags:: 

# 🌌 Course -> [[CSE 150B]]
---

# ❗ Motivation
- [[MTCS]] and all the recent advancements in Q Learning, etc., still cannot solve Sudoku
- Why? There is no heuristic we can rely on besides trying numbers
- Doesn't rely or depend on RL
- Structure of the space is different from the trees or $A^*$, branches, etc...
- Bottleneck for RL is that to solve, we need to explore the entire space, and when there are too many dimensions this fails
	- Not applicable in infinite number of spaces (continuous)
- We need a new perspective...

 
## ❗ Constraint Solving
- Abstract Idea:
	- Potential solutions form a space
	- The legal moves are defined by constraints on those variables
	- Solution is the point that satisfies the constraints
- 3 Part Framework:
	- Variables: $X = \{x_{1},\dots, x_{n}\}$
		- Things we can change / manipulate
	- Domains: $D = \{ D_{1}\times\dots\times D_{n} \}$
		- The space in which we can manipulate the variables
	- Constraints: $C = \{ c_{1}, \dots , c_{m} \}$
		- The constraints the variables must satisfy to count as a solution
	- Goal is to find an assignment of $X$ that satisfies all $C$
- ![[Pasted image 20240522181430.png]]
## Sudoku
- $X = \{ X_{1,1}, \dots X_{9,9} \}$
- $D = \{ 1,\dots,9 \}^81$
- $C=\{ X_{ij} \neq X_{kl} \}\cup \{ X_{ij} = a_{ij} \}$