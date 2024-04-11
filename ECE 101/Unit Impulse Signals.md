---
created:
  - 2024-04-10 23:46
tags:
  - ECE101
---
# ❗❓ Information
Related to:: [[Two Classes of Signals]]
Tags:: 

# 🌌 Course -> [[ECE 101]]
---

# Discrete Time Unit Impulse $\delta[n]$
- Definition: $\delta[n]=\begin{cases} 1, n=0 \\ 0, n \neq 0\end{cases}$
- Visual: ![[Drawing 2024-04-10 23.56.59.excalidraw]]
- We can express the unit impulse by shifting the unit step to the right by 1 and subtracting
	- $\delta[n] = u[n] - u[n-1]$
## Properties:
- Assuming $x[n]$ is a DT signal we have the following properties

[[Sampling Property]]
[[Sifting Property]]
[[Representation Property]]

# Discrete Time Unit Step $u[n]$
- Definition: $u[n]=\begin{cases} 1, n\geq0 \\ 0, n < 0\end{cases}$
- Visual: ![[Unit Impulse Signals 2024-04-10 23.59.41.excalidraw]]
## Ways we can express $u[n]$:

1. In terms of unit impulses by adding shifts of $\delta[n]$ together
	- $u[n]=\sum_{k=0}^{\infty}\delta[n-k]$
2. The "DT integral/Sum" of $\delta$ from $-\infty$ to $n$. 
	- If n is negative we sum up a bunch of zeros resulting in a 0. If n is positive or 0, we sum a bunch of zeros, the 1 at $\delta[0]$, and more zeros, resulting in a 1.
	- $u[n] = \sum^n_{l=-\infty}\delta[l]$
	- Visual: ![[Unit Impulse Signals 2024-04-11 00.15.05.excalidraw]]
3. A generalizable representation of $u[n]$ using the [[Representation Property]]:
	- $u[n] = \sum_{k=-\infty}^\infty u[k]\delta[n-k]$
	- Just the $\sum\delta[n-k]$ portion is just the unit impulse from $-\infty$ to $+\infty$, giving us stems with magnitude 1 across the board.
	- Sum of all shifted unit impulses from $-\infty$ to $\infty$:![[Unit Impulse Signals 2024-04-11 00.37.26.excalidraw]]
	- We multiply these terms with the coefficient of the actual value of $u[k]$ from $-\infty$ to $+\infty$:![[Unit Impulse Signals 2024-04-11 00.40.36.excalidraw]]
- **This will generalize to arbitrary $x[n]$**
		- $x[n] = \sum_{k=-\infty} ^\infty x[k]\delta[n-k]$
		- "Builds the signal one stem at a time"![[Unit Impulse Signals 2024-04-11 00.43.45.excalidraw]]
	- This is the intuition for the [[Representation Property]]

