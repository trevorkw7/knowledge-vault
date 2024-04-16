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
### Sampling Property of $\delta[n]$
> [!note] Discrete
> - $x[n]\delta[n] = x[0]\delta[n]$
> 	-  Multiplying DT signal $x[n]$ by the unit impulse results in a new signal that's simply an impulse at 0 with the magnitude of $x[0]$
> - $x[n]\delta[n-n_{0}] = x[n_{0}]\delta[n-n_0]$
> 	- Multiplying the DT signal by a time-shifted unit results in a new signal that's simply the impulse at $n_{0}$ with the magnitude of $x[n_{0}]$

### Sampling Property of $\delta(n)$
 > [!important] Continuous 
 > Mathematically: $x(t)\delta(t-\tau)=x(\tau)\delta(t-\tau)$
 > 
> If we multiply a signal x(t) with $\delta(t-\tau)$, which is just a impulse located at $\tau$, x(t) gets "sampled" at $x(\tau)$, which is the impulse at $\tau$ with magnitude $x(\tau)$
