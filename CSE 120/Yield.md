## "The Magic of Yield"
![[Pasted image 20240110190521.png]]
- When we saved the PC (program counter) it was pointing to the next line `if (magic == 1) return;`
- asm restore PC will jump back to that line
- On first glance, it looks like magic will never == 1 so we can remove it. This is WRONG

## Yield Example 1
![[Pasted image 20240110191455.png]]
- Assume process A is running
	- At some point B must've yielded to A in the past
- `SaveContext (me)` is an assembly macro

## Uncovering the Magic
![[Pasted image 20240110191914.png]]
- PC points to the process of whatever is currently running, we start with process A
- SP begins with pointing to the top of the empty stack
- Getpid () gets put on the stack and popped off the stack returning it the name of the current process to the local variable `A`
- Yield(B) is a function which creates an activation record, it creates an an activation record that returns to the the second yield Yield(A)
- Inside Yield(B), we set magic = 0 in this activation record and we save the context to a shared memory 


## [[Yield via Kernel]]