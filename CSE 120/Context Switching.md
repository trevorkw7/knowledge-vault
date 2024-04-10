## Definition
- Allocating CPU from one process to another
## Method
1. Save [[Context]] of currently running process (registers, stack pointer, etc.)
	- Save registers
	- Switch text and data
	- Switch stacks
2. Load [[Context]] of new process 
- When this happens we are in [[Yield]]