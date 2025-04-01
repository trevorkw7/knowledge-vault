![[Pasted image 20240110184841.png]]
- The activation record contains a link/pointer to the previous record that's used when **return** is called
	- Specifically the hardware register "SP"
- All local variables go inside the activation record
- The activation record stack holds records for all pending processes, completed processes are removed from the stack