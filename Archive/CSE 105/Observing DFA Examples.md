1. ![[Pasted image 20231022000132.png]]
	- must start with aab to reach accept state after which we just use b's
	- must start with 2 as, must end with b 
	- Regex Expression: $L(aa^*bb^*)$
	- Answer: C
2. ![[Pasted image 20231022214915.png]]
	- Answer: B
	- 1st state is for when a has not yet appeared, 2nd state is for when b's followed by a, q3 is for after seeing the pattern ab
3. ![[Pasted image 20231022215458.png]]
	- Answer: q1 (because if a occured would automatically move to q2 so only strings that end here only have bs), q2 (because if b occured here after the a's, it would go to q3): $\{ q_{1}, q_{2} \}$
		- Note: Empty string avoids a,b so should be accepted