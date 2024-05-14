## Attention is all you need
- Proposed the transformer architecture
- Authors didn't anticipate the impact on the field so it reads a lot like a normal paper
## Dataset
- Andrej Karpathy uses a shakespeare dataset
- We will use speeches from 3 American politicians
## Nano GPT
- Repository for training transformers
- Simple implementation
- `model.py` - defines the GPT model
- `train.py` - reproduces GPT-2

# Steps

## Step 1: Dataset Import
- Open a text file and read it in
- In Andrej's video he uses shakesphere, in our transformer model we will use 3 presidential speeches
## Step 2: Tokenization
- For storage, we need to encode characters / words into a list of integers
- Some common approaches in industry are:
	- Sentence Piece - uses sub-word units
	- Tik Token - byte pair
- There is a tradeoff between the codebook size and the sequence length
	- Short sequences of integers with long vocabularies
	- Long sequences of integers with short vocabularies
- For the purposes of building a simple GPT, we will map the set of characters to integers and encode individual characters -> lists of integers
## Step 3: Train/Val Split
- We first encode our entire dataset using the tokenization system in step 2 and and place it into a pytorch tensor
	- This looks like just a long sequence of integers
- We use a 90% train 10% validation split:
	- `n = int(0.9 * len(data))`
	- `train_data[:n]`
	- `val_data[n:]`
## Step 4: Data Loading
- To feed the text sequences into the transformer for it to learn, we need to sample small chunks from training set of a set length, a.k.a:
	- block size
	- context length
	- etc..
- This is because training on the entire dataset at once is too computationally intensive
- Additionally blocks will help the transformer get used to seeing contexts from as little as 1 all the way to block size x
- Each "block" that we feed to the transformer with length x trains the transformer on x-1 examples:
	- block = [18, 47, 56, 57]
	- when input is 18, the target is 47
	- when input is 18, 47, the target is 56
	- when input is 18, 47, 56, the target is 57
	- etc...
- For efficiency, instead of processing one sequence at each time, we process batches which contain multiple independent sequence for GPU parallel processing
- Visualized and spelled out:![[Pasted image 20240513192628.png]]