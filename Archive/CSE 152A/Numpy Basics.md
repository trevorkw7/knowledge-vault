
## Arrays
- Create an array: `np.array([1,2,3])`
- `.shape` returns the number of elements in 1st dimension followed by 2nd etc.
- The first dimension counts how many elements are in the outermost row, second on the inside of each of the inner arrays, etc.
- Useful commands for creating matrices:
	- `.zero`
	- `.ones`
	- `.eye`
	- `.random.rand(2,3)`
## Array Indexing
- Indexing works by finding nth element of `[first dimension, second dimension]`
- Accessing subarray:
	- Individual row or column: `m[1,:]`, `m[:,1]`
	- Submatrix `m[1,start:stop]`
		- Note stop isn't included only goes up to stop, not including stop goes to the end
- Replacing subarray:
	- Replace column: `m[:,0] = np.array([1,1,1])`
	- Replace row: `m[0] = np.array([1,1,1])`
	- Replace submatrix: `m[:2, :2] = `
		- This would replace a 2x2 submatrix with another 2x2 submatrix
## Array Transposing
- Transposing a 1d array doesn't do anything `m[1,:]` is the same as `m[1,:].T`
- To manually change order of axis / dimensions use: `np.transpose(m[1:, :], axes=(1,0))`
## Reverse order of subarray
- Use slice notation and make the increment -1
- `m[1, ::-1]`
## Boolean array indexing
- `m[m>0]` returns a list of all indices where m>0 as if everything was indexed in 1 long list
- Can use this to tricks like replace everything greater than 2 with 0: `m[m > 2] = 0`
- Advanced modify array with another array based on boolean expression:
```
- m = np.array([[1, 2, -3], [4, -5, 6]])
n = np.array([[1, 10, 100], [1, 10, 100]])
n[m > 0] = m[m > 0]
print("\nBoolean array indexing: Modify with another array")
print(n)
```

## Reshape Command
- Reshapes the current data into m.shape(# of layers, # of rows, # of columns )
- Layers are represented by an extra bracket, so a (2,2,1) would have 2 layers 2 rows 1 col: ![[Pasted image 20240119133522.png]]
- Stack: takes 2 matrices and puts the first one at layer 0 and the second one at layer 1 (`np.stack((m1,m2))`)
- Concatenate: Within 1 layer / 2 dimensions it takes the 2 matrices and sticks them together by adding extra rows by default. If you pass in axis=1 it sticks them by column. 
	- By Row
	- ![[Screenshot 2024-01-19 at 1.40.10 PM.png]]
	- By Col (np.concatenate((m1,m2), axis=1)):
	- ![[Screenshot 2024-01-19 at 1.41.39 PM.png]]
## Sum and Mean
- Pretty self explanatory
```
a = np.array([[1, 2, 3], [4, 5, 6]])
print("Sum of array")
print(np.sum(a))                # Sum of all array elements
print(np.sum(a, axis=0))        # Sum of each column
print(np.sum(a, axis=1))        # Sum of each row
print("\nMean of array")
print(np.mean(a))               # Mean of all array elements
print(np.mean(a, axis=0))       # Mean of each column
print(np.mean(a, axis=1))       # Mean of each row
```

## Dot products
```
a = np.array([[1, 2], [3, 4]])
b = np.array([[1, 1], [1, 1]])
print("Matrix-matrix product")
print(a.dot(b))                 # Matrix-matrix product
print(a.T.dot(b.T))

x = np.array([3, 4])  
print("\nMatrix-vector product")
print(a.dot(x))                 # Matrix-vector product

x = np.array([1, 2])
y = np.array([3, 4])
print("\nVector-vector product")
print(x.dot(y))                 # Vector-vec
```
## Matplotlib Boilerplate
```
%config InlineBackend.figure_format = 'retina' # For high-resolution.
import numpy as np
import matplotlib.pyplot as plt

x = np.arange(-2., 2., 0.01) * np.pi
plt.plot(x, np.sin(x))
plt.xlabel('x')
plt.ylabel('$\sin(x)$ value') # '$...$' for a LaTeX formula.
plt.title('Sine function')

plt.show()
```