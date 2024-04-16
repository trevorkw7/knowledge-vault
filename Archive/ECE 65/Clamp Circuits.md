

![[ECE 65 Lecture 9.pdf]]

### Summary
- Quick way to remember whether the DC shift is positive or negative
	- Diode facing down -> negative
	- Diode facing up -> positive
- Reading Quiz Notes:
	- Seeing the output we can tell that its a clamp circuit because of the DC shift down![[Pasted image 20231018140848.png]]
	- We also add a $V_{dc}$  source under the diode so we can adjust the DC shift
		- Note: in this example $V_{DC}$ is 2V
	- Characteristics of this circuit:
		- For $0 < V_i < 2$ the diode is off and $V_C = 0$ 
		- When $V_i > V_{DO} + V_{DC} = 2V$,  $V_D > 0.7V$ which turns the diode on
		- After $V_i$ reaches it's peak amplitude, the diode turns off because $V_c = V_i$ 
			- $V_o = V_i - (V_p - V_{dc} - V_{DO})$  

### Discussion question 1
- Design: ![[Pasted image 20231018142523.png]]
- We want $V_{out}$ to have a 5V DC shift compared to $V_{i}$ : $V_o = V_i  + 5$ 
- KVL tells us that $V_c = -V_p + V_{DC} + V_{D0}$
- $V_o = V_i  + (V_p - V_{DC} - V_{D0})$  
- $5 = (10 - V_{DC} - 0.7)$ 
- $V_{DC} = 10 - 0.7 - 5 = {4.3}V$ 
- Circuit Charactaristics:
	- When the diode is on, $V_c (t) = V_c(t) V_{dc} + V_{D0}$ 
	- Then Vi reaches its peak negative amplitude and the diode will stop conducting
	- $V_c = -V_p + V_{dc} + V_{DO}$ 
	- $V_c$ is now constant from this point onwards so our $V_o = -V_c + V_i = V_i - (-V_p  + V_{DO} + V_{DC}) = V_i - (-10 + 0.7 + V_{dc})$  

### Midterm Notes
- Bring circuit drawings of all the structures we learned for the different circuits: clipper/clamp/etc