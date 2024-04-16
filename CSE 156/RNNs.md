---
created:
  - 2024-04-10 23:46
tags:
  - CSE156
---

# ❗❓ Information
Related to:: 
Tags:: 

# 🌌 Course -> [[CSE 156]]
---

# ❗ RNNs = Unrolled Recurrent Neural Networks
- Core Idea: Apply the same weights W repeatedly
- Condition the next word on the entire sentence history instead of a fixed-size window
- Variable length data leads to **variable number of parameters**
- RNN gives me a vector that can predict next word
- NOT a language model

 
## ❗ Advantages
- Can process any length input

## Fancy RNN Variants
- [[Bidirectional RNNs]]
- [[Multi-Layer RNNs]]
- [[LSTM RNNs]]
- GRU