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

# ❗ CT Transform
- Idea: Takes a signal and gets a representation in the frequency domain
- Works for aperiodic signal
- Synthesis Equation:
	- Tells how to get the signal from the transform
	- $x(t) = \frac{1}{2\pi}\int _{-\infty}^\infty X(jw)e^{jwt}\, dx$
	- Sums up all the frequencies 
	- $X(jw)$ acts to replace $a_{k}$
	-  Comparison to periodic signal synthesis equation:
		- $x(t) = \sum_{k=-\infty}^\infty a_{k}e^{ykw_{o}t}$
		- Only has frequency content and we sum it up
- Analysis Equation:
	- $X(jw)=\int _{-\infty}^\infty x(t)e^{-jwt}\, dt$
	- Integral over time domain
	- Comparison to periodic signal analysis equation:
		- $a_k = \frac{1}{T} \int_{0}^{T} x(t) e^{-j k \omega_0 t} dt$
		- The counterpart to $a_{k}$ if FT is $X(jw)$, which is continuous instead of discrete since we extend period $T$ to infinity
## Requirements
- Doesn't need to be finite duration 
- $\int _{-\infty} ^{\infty} \mid x(t)\\^{2}\mid \, dt < \infty$
	- Integrating magnitude of the signal squared has to be finite: Energy Must be **FINITE**
		- Decaying exponentials work, but if it heads to infinity like increasing exponentials, it won't work
	- For LTI systems, $H(jw)$ (the CTFT of $h(t)$) is well defined if $\int _{-\infty}^\infty \mid h(t) \mid^{2} dt < \infty$
- OR Dirichlet conditions
	- 1. $x(t)$ is absolutely integrable: $\int _{-\infty}^\infty \ |x(t)| dt < \infty$
	- 2. Has an finite number of maxima and minima for any given time interval
		- Too many oscillations don't work
	- 3. Has finite number of discontinuities within any finite time interval
	- IF all of these conditions hold then $X(jw)$ exist and $\hat{x}(t)$ which is the result of using the analysis equation $x(t) \to X(jw)$ followed by the synthesis equation $X(jw) \to x(t)$ satisfies these conditions
		- At points of continuity $\hat{x}(t) = x(t)$
		- At points of discontinuity, $\hat{x}(t)=$ average of values on either side
 
## ❗ Derivation
![[Pasted image 20240521232400.png]]
- Following this derivation for X(jw), replace the F.S. coefficients $a_{k}$ with $X(jw)$ which is a cont. function. Since its cont. we need to do an integral instead of sum.