---
created:
  - 2024-05-29 23:51
tags:
  - CSE150B
---

# ❗❓ Information
Related to:: 
Tags:: [[Continuous Time Fourier Transform]]

# 🌌 Course -> [[CSE 150B]]
---

# ❗ Overview
- Use case: To convert signals from time domain to frequency domain that have infinite energy
- Example: ![[Pasted image 20240529235402.png]]


### Definition
![[Pasted image 20240529235653.png]]
- ROC / Reigon of Convergence is the range for $s$ in which $X(s)$ exists 

### Relation with [[Continuous Time Fourier Transform]]
- $s=\sigma + j\omega$
	- $\sigma$ is the real part of the complex variable $s$
- If we substitute $s =\sigma +j\omega$ , we actually arrive on a form in this integral that resembles the definition of CTFS as seen below: ![[Pasted image 20240530001317.png]]
- Since [[Laplace Transform]] is a subset / form of CTFS, we can say that:
	- If the **Laplace Transform** $X(s)$ exists, then the CTFS 
## ❗ Answer