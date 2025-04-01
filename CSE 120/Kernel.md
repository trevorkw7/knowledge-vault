- Exists in the middle between running programs and hardware
- ![[Pasted image 20240109014647.png]]
- Has 2 interface:
	- green is for programmer
		- goals: simplicity, convenience
	- red is for hardware
		- goals: performance, reliability, security
- At a high level: makes machine easier to use by creating illusion that there is unlimited processors and memory, programmer can focus on solving the problem
- Most basic kernel function: **run a program**
	- We can do even better: run multiple programs with a single CPU + memory
- Runs as an extension of all [[Process]]es

## Three Key Ideas for OS
[[Abstraction]]
[[Mechanism]]
[[Policy]]

## Detailed Anatomy
- Contains text, data, and multiple stacks
- The saved contexts for when context switching occurs exist in kernel data
- The yield routine is stored in the kernel text