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
- When a system is **[[Additive]]** and **[[Scalable]]**
- In linear systems, if input signal $x(t) =0 $ is applied to the system, the output will be $y(t) = 0$ 
- Equivalent condition: linear superposition holds

 
### ❗ To check for Linearity of a System
Given $x[n]$
1. Define new signal $x_{3}[n] = ax_{1}[n] + bx_{2}[n]$
2. Find system response when $x_{3}[n]$ is our input into the system: $y_{3}[n]$
3. Find scaled and shifted version of $y[n]$: $y_{4}[n] = ay_{1}[n  ] + by_{2}[n]$
4. Compare $y_{3}[n]$ and $y_{4}[n]$, if equivalent the system is linear
### Examples
1. ![[Pasted image 20240418021004.png]] Answer: Not linear because scaled and shifted signals don't hold shown in #4