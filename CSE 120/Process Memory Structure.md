## Consists of...
- Text
	- Code / program instructions
- Data
	- Global variables
	- Heap (malloc, dynamic allocation)
- Stack
	- [[Activation Record]]/Stack Frames
		- All information about the procedure that was currently called
		- When procedure returns it's popped of the stack
	- Automatic growth/shrinkage
	- Provided as part of the operating system to allow your program to run
	- [[Detailed Look at Process Stack]]
	- At any point in time, the uppermost activation record is the most relevant as it contains the information of the current procedure / function the process is executing. Thus the [[Stack Pointer]] is dedicated to pointing to it

## Contained between 0 and N-1
- In terms of addresses
- ![[Pasted image 20240110184302.png]]
- Data and Stack shouldn't collide because of how much space there is, however still theoretically possible