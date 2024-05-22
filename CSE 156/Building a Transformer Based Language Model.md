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
- This means our vocab size is equal to length of the set of unique characters: [a,b,c,d,e,...] and this will also be our embedding length 
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
## Bigram Model 
- Simplest language model that predicts the probability of a word based on the previous word
- Implemented by creating a subclass of nn.Module
- We pass the inputs and targets, which we define from data loading above
- The constructor creates a "token embedding table" with vocab_size x vocab_size because the table is a matrix with dimensions **vocabulary size x embedding dimension**, which maps each token (word) in the vocabulary to a corresponding vector of logits, which are used to predict the next token in the sequence.
- In the forward pass, we take in `idx` which is the tensor of  the shape `B,T` where B is batch size and T is sequence length. Idx in this case is the given sequence that we want to predict the next word for. 
- The output `logits` has dimension `C` which is the embedding dimension which is the same as vocab size.
	- example: if our input text only had characters a,b,c,d, then our embedding size = vocab size = 4, so output logits would look like [0.3, 0.4, 0.1, 0.8] which are confidence measures of what character from our vocab is predicted to appear next
- We measure loss as the cross entropy between the **logits**, which are the predicted outputs, and the **targets**, which is the actual output
- Tokens don't talk to each other, we only look at last character when making prediction

## Self Attention Block
- Mathematical Trick in Self-Attention:
	- Token should only communicate with previous timesteps
	- For a tensor with batch_size = 4, time = 8, channel = 2
	- For each batch element, for every Tth token, we calculate the average for all the previous tokens and the current one, known as "weighted aggregation"
	- This is inefficient so we can use matrix multiplication to speed this up
		- a= $\begin{matrix}1,0,0 \\ 1, 1, 0 \\ 1,1,1 \end{matrix}$
		- $b = \begin{matrix}2, 7 \\ 6, 4\\ 6, 5\end{matrix}$
		- If we multiply a x b, then we get c = $\begin{bmatrix}2 , 7 \\ 8, 11, \\ 14, 16\end{bmatrix}$
		- Here, value at the row and col of c is equal to the sum of the previous and current values in the columns of b
		- If we normalize a so that the rows sum up to 1: $\begin{bmatrix}1,0,0 \\ 0.5, 0.5, 0 \\ 0.33,0.33,0.33 \end{bmatrix}$ 
		- c will give us our average
	- We implement this with `torch.tril` and `masked_fill` and `softmax` to create oru weighted matrix and multiply it with 
		- Future tokens are set to negative infinity
		- Previous values are interested in each other, how interested they are is determined by "affinities"
## Self Attention
- Every single token at each position will emit 2 vector:
	- query: what am i looking for
	- key: what do i contain
	- value: another representation of x (contains all the tokens in different batches) that is used for the weighted sum calculation
	- All the tokens in all the positions in the B x T arrangement independently and in parallel produce a key and query![[Pasted image 20240515023440.png]]
- Affinities between tokens are a dot product between the keys and queries
- This becomes the weights for the weighted average at time t
- `wei = q @ k.transpose(-2, -1) # (B, T, 16) @ (B, 16, T) ---> (B, T, T)`
- Effect: If affinities between the current t's query and a previous t's key are similar, the weighted average will contain more data on the that previous t
## Encoders and Decoders
- Encoder: We might not always want to mask future nodes / tokens since for sentiment analysis we want the full picture
	- Simply remove the masked fill
- Decoder: Keep the masked fill

