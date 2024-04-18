---
created:
  - 2024-04-10 23:46
tags:
  - ECE101
---

# ❗❓ Information
Related to:: [[System Properties]]
Tags:: 

# 🌌 Course -> [[ECE 101]]
---
## ❗ Defintion
- For all all inputs $x(t)$ and all time shifts $t_{0}$ the output to $x(t-t_{0})$ is $y(t - t_{0})$
- Response of the system is not time dependent

 
### ❗ To check for TI Property
Given $x[n]$
1. Define new signal $x_{1}[n] = x[n-n_{0}]$
2. Find system response $x_{1}[n]$ as our input into the system: $y_{1}[n]$
3. Find shifted version of $y[n]$ by $n_{0}$: $y[n-n_{0}]$
4. Compare $y_{1}[n]$ and $y[n-n_{0}]$

### ❗ Example
1. Is $y(t) = \sin(x(t))$ TI? 
	- $x_{1}(t) = x(t-t_{0})$
	- $y_{1}(t) = \sin(x_{1}(t)) = \sin(x(t-t_{0}))$
	- $y(t-t_{0}) = \sin(x(t-t_{0}))$
	- Comparing $y_{1}(t) = y(t-t_{0})$, these are the same, thus this is TI
2. Is the system $y[n] = nx[n]$ TI?
	- $x_{1}[n] = x[n-n_{0}]$
	- $y_{1}[n] =  nx_{1}[n] =nx[n-n_{0}]$
	- $y[n-n_{0}] = (n-n_{0})x[n-n_{0}]$
	-Comparing $y_{1}[n]$ and $y[n-n_{0}]$ these are not the same, not TI