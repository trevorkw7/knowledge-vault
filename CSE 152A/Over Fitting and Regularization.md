## Overfitting
- Suppose we only use 1000 instead of 60000 training images
- We can do well on the training data but when presented with unseen training data the model performs bad
- Overfitting: Model finds shortcuts in its training data which means it doesn't end up generalizing well
- Simple solution: Just use more data yay!
- When we don't have more data we can limit model complexity using **regularization**

## Regularization 
- Ensure model is not too complex by using L2 regularization, L1 regularization
- "Smooths out weights" by making them more similar and decrease the deviation of the weight values
- This makes them less sensitive to small changes in input data
- L1 Shrinks weights by a constant amount towards 0
	- "Sparsifies the weights"
- L2 Shrinks an amount that is proportional to w