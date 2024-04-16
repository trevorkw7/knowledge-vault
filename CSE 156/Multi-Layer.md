---
created:
  - 2024-04-10 23:46
tags:
  - CSE156
---

# ❗❓ Information
Related to:: 
Tags:: [[RNNs]]

# 🌌 Course -> [[CSE 156]]
---

# ❗ Idea
- Aka stacked RNNs
- We have multiple RNN layers and the hidden states from each RNN layer i are the inputs to the next RNN layer it feeds to i + 1: ![[Pasted image 20240416104138.png]]

 - In practice, high performing RNNs are often multi layers
 - Learning more and more complex features 
 - BERT for example has up to 24 layers, which is **transformer-based** network
 - Middle Layers are more multi purpose
 - Last Layers are more task specific for whatever are retrained for