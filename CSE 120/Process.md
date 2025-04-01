- Related to [[Context]] which is all of the state describes a *process* in a particular point in time
- [[Process Memory Structure]]
## Definition
- [[Abstraction]] of not a program (list of instructions) but a program in execution
- Is dynamic, has state, and changes unlike a program which is static
	- Formal Definition:A set of state variables and their values at each point in time for the duration of a running programming
	- Analogy: Program is recipe, process is cooking 🧑‍🍳
## To Support the Process Abstraction, we need  **Resources**
- [[Resources]]
 - CPU
	 - Processing cycles
	 - **Executes instructions**
 - Memory
	 - Bytes or words to **maintain state**
	 - [[Process Memory Structure]]
 - Other Resources
	 - I/O like printer, network, display, etc.

## Supporting Multiple Processes
- Most processes are waiting instead of running
- [[Multiprogramming]]
- 

- anything that describes what the process is doing at a given moment of time (stack pointer, frame pointer, general, program counter)