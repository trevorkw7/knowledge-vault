### Example 1:  Does a specific DFA accept a given string?
- Define a Turing machine of $M =$ "On input x
	- Type check encoding to check input is valid type $<B, w>$"
	- Simulate B on input w
	- If the simulation ends on accept state of B, accept, if it ends on non-accept state of B reject
- This works because DFAs always end in accept or reject
- Turing machine $M$ is a decider and $L(M)$ is decidable
- 