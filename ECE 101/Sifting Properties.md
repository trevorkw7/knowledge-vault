---
created:
  - 2024-04-10 23:46
tags:
  - ECE101
---
	
# ❗❓ Information
Related to:: [[Discrete Time Unit Impulse Signals]]
Tags:: 

# 🌌 Course -> [[ECE 101]]
---
### Sifting Property of $\delta[n]$

> [!note] Discrete
> $\sum_{n=-\infty}^\infty x[n]\delta[n] = x[0]$
> - $\sum_{n=-\infty}^\infty x[n]\delta[n-n_{0}] = x[n_{0}]$ 
> - Idea: Summing over the signals created by the sampling property $x[n]$ gives us just the value where we "sample" $x[n]$

 > [!important] Continous
 > $\int_{-\infty}^\infty x(t)\delta(t-\tau) \, dt = x(\tau)$
> - Idea: Integrating over $x(t)\delta(t-\tau)$ which is the signal created by the continuous sampling property from $-\infty$ to $\infty$ is equal to $x(\tau)$  which is where we "sample" $x(t)$

