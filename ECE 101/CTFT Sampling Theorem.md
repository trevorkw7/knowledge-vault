---
created:
  - 2024-04-10 23:46
tags:
  - ECE101
---

# ❗❓ Information
Related to:: 
Tags:: 

# 🌌 Course -> [[ECE 101]]
---

# ❗ Utility
- Can a CT time signal be reconstructed from sampled version of the signal?
- Yes! 
	- Provided that the signal is **band limited**
		- **band limited** means there is a maximum frequency
	- Sampling rate must be at least 2 times the maximum frequency 
- Idea: Take a CT signal and to convert it to a train of CT impulses. Height of these impulses are the sampled values
	- How? Sampling property
		- Impulse Train Sampling System: ![[Pasted image 20240522012318.png]]
		- We sample every T seconds
		- Simply multiplying our signal by $p(t)$ will give us our discretized version of $x(t)$
		- Mathematically
			- $x_{p}(t) = x(t)p(t) = x(t)\sum_{n=-\infty}^\infty\delta(t-nT)$ 
			- $=\sum_{n=-\infty}^\infty x(nT)\delta(t-nT)$
		- This exactly a train of impulses bounded by the envelope $x(t)$ with distances $T$ x

 
## ❗ Answer