## 5 Stage Pipeline
**F - Fetch**
**D - **
**X - eXecute**
- By the end of this cycle the execution has finished
**M - **
**W - write to register**

### Hazards
- Data Hazard: 
	- Need to stall in DECODE stage (D)
	- If we have two insructions that require dependencies
	- W has to happen (writing) before we use the dependency in the next instruction
- Structure hazard:
	- Stall in Fetch stage (F)
	- Is a hardware conflict, for example when two instructions try to occupy the same components (ex: decode stage)


## Bypassing
- MX Bypass
	- Read the value after execution in the first instruction from the temporary register (M) and routes it back so that the execution of the second instruction can happen 
- WX Bypass
	- When there's a gap between the two instructions 
	-  Forward from beginning of W stage to X stage