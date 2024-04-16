## Assumptions
- Convolutions are done with padding, effect of edge values is small

## Special Case
- 1X1 Convolutions are used to change channel depth 

## Overview
- We have convolutional layers and create feature maps (much smaller dimension than input image)
- At the end we connect a few fully connected layers and end with a loss function
- Input: Image -> Convolutional Layer -> Pooling Layer -> Flattening (Vectorized version of 3d tensor from convolutional layer) -> Neurons connected though fully connected layers -> 2 Activation Neurons (Dog vs Cat)
- All operations are matrix vector products
- Local Connectivity: Same local functions evaluated everywhere
- Weight Sharing: Much fewer parameters
- Pooling: Larger "Receptive Field"
- Limit Parameters: 3x3 filters instead of larger image filters
- 1x1 Convolutions to reduce dimensions
- Skip Network: Easier optimization with greater depth (RESNET)
- Dimensionality is constrained how many inputs we expect for fully connected layers
	- Thus we need to resize our training images so they're all the same size

## Loss Function
- How do we know whether the unbounded output for the neuron is relatively big or small
- Answer: Softmax $f_{j}(z) =\frac{e^{z_{j}}}{\sum_{k}e^z_{k}}$
- Softmax converts the raw output scores into into probabilities by normalizing from 0 to 1
- Mathematically this is done by taking the exponential of each output and dividing by the sum of all the exponentials
- $\mathbb{n}$

[[CNN Architectures]]
