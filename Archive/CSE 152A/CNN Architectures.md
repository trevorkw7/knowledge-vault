## Regularization Techniques

L1
- Sparsity, push weights close to 0
L2
- Normalize weights by reducing difference between each rate
Dropout
- Works because the network is "lazy", so it will take shortcuts that may not be robust to different training images
- Forces neurons to learn independent of others
Data Augmentation
- Change color values, contrast, brightness etc. 
- Empirical problem to find best strategy (try a bunch)

## AlexNet
- Most used and famous

## VGGNET
- Much more accurate than alexnet
- More than twice as many layers which allows for the learning of features to be more abstract
- Harder and slower to train
- Exploding / Vanishing Gradients because depth with backpropgation makes training hard if one of the gradients are either really small or really big
## ResNet: Its deep
- Stands for residual net
- Adds a identity mapping between the input and output of a layer
- Solves the problem of exploding / vanishing gradients and allows network to go deeper
- 
