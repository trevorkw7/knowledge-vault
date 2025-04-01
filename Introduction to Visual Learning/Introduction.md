### Resources
- Wednesday OH are usually for learning jupyter notebooks
- Monday OH for others
- 2 TAs
### Prerequisites
- Python
- Linear Algebra

### Final Project
- Goal is to experiment and implement something new / novel

### What is Learning?
- No longer limited to searching in databases, but now have power to generalize
- In computer vision you have training data and test data, performance on test data is key


### History of Facial Recognition
1. Hand crafted features to do sliding window over pixel values (2001) 
2. Measure gradients / difference in intensity between pixels to calculate histogram, learn template using structured vector machines, then use sliding window until we find location which has highest response to template, goal was to build global human classifier which was **1 layer**(2005)
3. Deformable part-based models to build templates for torso, face, etc. Distance between each one of these boxes threshold is learned. Uses **two layers**, the root filter which represents the overall object appearance and the individual part filters  (2009)
4. Introduction of many layers that are learned, several hundreds, using CNNs and deep learning trained through back propagation instead of training each layer of classifier individually(2012)

## Types of Deep Networks
### Multilayer perceptron (MLP)
- Input: 1024 pixels
- Each pixel has 2000 parameters tuned to transform it
- We get 1024 X 2000 parameters total
- Completely data driven, lots of parameters
### Convolutional Neural Network (CNN)
- Idea is there should be generalizability, there are visual patterns that are repetitive this should save us parameters
### Transformers
- With the introduction with transformers, we have thrown away the ideas of CNNs and with enormous data we throw away the prior and have gone back to training MLP from scratch which yields better performance
### In Summary
- We continue to throw away prior work and keep moving towards pure data driven


# Problem Topics Covered in Class

## Perception Topics
- Image captioning
	- Initially worked on in 2015
	- With the rise of LLMs it has resurged
- Object detection and segmentation
- Human pose estimation
## Image Generations
- GANs (2018-2022) - using a model to generate an image or data that aligns with the distributions
- Diffusion models (2023-present)
- Recurrent neural networks (2025-present): large language models are now generative images
### 3D
- 3D mesh reconstruction with images
- Implicit representation with NeRF
	- Realize this is not scalable
- Now we are going back full circle back to 3d mesh reconstruction
### Video
- Lot's of recent progress with video generation (SORA)
- Physical interaction prediction 