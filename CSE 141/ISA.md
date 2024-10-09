
### Program Execution model vs Instruction Execution Model
- We mainly care about instruction execution model
- Program is just a set of instructions

## CISC vs RISC
- Mainly talk about RISC
- RISC -> reduced, simple instructions
	- Software development harder because each instruction accomplishes very little, hardware implementation easier
- CISC -> complex
	- Software development easier because on instruction accomplishes more, hardware implementation more difficult
	- Larger die area, less energy efficient

## Aspects of ISAs

![[Pasted image 20241008130952.png]]
- Length
	- Fixed, most commonly 32 bits
- Encoding
	- Machine code (1s and 0s) <-> assembly
	- Example: MIPS
		- Fixed length, 32 bit
		- R type: register operations
		- I type: immediate values like memory access, branching
		- J type: jump
- Datatypes:
	- Software: attribute of data
	- Hardware: attribute of operation, data is encoded into 0/1s
	- Lives in registers *(R0, R1, F0)*, memory *(R3, R5)*
		- registers are faster because there are fewer of them 
			- can't put structures and arrays
		- memory is slower, long term
- Addressing:
	- Way of specifying memory address *(R3, R5, etc.)*
	1. Displacement: Addressing where address of data is calculated by adding a fixed number to the value in a register
		- This is done in MIPS because research on VAX which supports many addressing modes found that 80% of memory access uses small displacements and 1% uses a displacement larger than 16 bits. This means most memory accesses are near data already in registers
	2. Absolute: data is located at fixed memory address, zero + offset
	3. Register indirect: address to memory is stored in register
	4. Indexed: use two registers and address is sum of values in both
	5. Scaled: one register is multiplied by a scale factor (*R2 * Scale*) + offset (*R1*)


## ISA Exercises
![[Pasted image 20241008132620.png]]
1) Calculate the total number of data memory accesses made during execution of the code.
	1. I type, no access
	2. R type, no access
	3. I type, accessed word which is in memory +1 (load))
	4. R type, no access
	5. I type, accessed word in memory +1 (load)
	6. R type no access
	7. R type no access
	8. I type, store word which is in memory +1 (sotre)
	9. I type, no access
	10. I type, no access
	11. I type, no access
		Answer: 3


2) 3 * 2 loads + 2 * 1 store +1 * 8 other = 6 + 2 + 8 = 16 cycles
- numbers of instructions: 11
- CPI = number of cycles / instructions executed 16/11 = 1.45

3) C * 500ns = 8000ns = us
