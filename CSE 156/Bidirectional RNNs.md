---
created:
  - 2024-04-10 23:46
tags:
  - CSE156
---

# ❗❓ Information
Related to:: [[RNNs]]
Tags:: 

# 🌌 Course -> [[CSE 156]]
---

# ❗ Idea
- Gives the contextual representation of a word in a sentence with right and left context: ![[Pasted image 20240416102651.png]]
- The "hidden state" of the bidirectional RNN, which is what we pass onto the next parts of the network is composed of the Forward RNN $RNN_{FW}(\vec{h}^{t-1}, x^t)$ and Backward RNN $R\mathbb{N}_{BW}(\vec{h}^{t+1}, x^t)$ 
- Only applicable if you have access to the **entire input sequence
	- Thus not applicable in LM because we only have left context available
- We can also stack RNNs

