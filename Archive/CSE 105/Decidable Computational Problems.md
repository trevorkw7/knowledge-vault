## Decidable Computational Problems
- $A_{DFA}$ is decidable and recognizable because all DFAs either reject or accept
- $E_{DFA}$ is decidable ($L(M_{2}) = E_{DFA}$ and $M_{2}$ is a deicider)
	- Construction: 
		- can create a a TM $M$ = on input x"
		- type check to see if x is an encoding < A > such that A is a DFA. if not return false"
		- run BFS on the start state of A
			- Mark the start state of A visited
			- Loop over states of A and mark any unmarked state that has an **incoming edge from a visited state**
		- if any accept states are visited then return false
		- else return true"
	- Note: since DFA, BFS is will halt
	- Proof of Correctness: $L(M_{2}) = E_{DFA}$
		- Show a language of a machine is equal to a language by showing
			1. $L(M_{2}) \subseteq E_{DFA}$ 
				- Means $x \in L(M_{2}) \rightarrow x \in E_{DFA}$
				- Contrapositive: $x \notin E_{DFA} \rightarrow x \notin L(M_{2})$
				- Proof by contradiction:
				- Assume that $x \notin E_{DFA}$
				- Case 1: The input $x$ is not a valid encoded DFA. 
					- It fails $M_{2}$'s  type check so $M_{2}$ will reject and $x \notin L(M_{2})$
				- Case 2: The input $x = <M>$ is valid and $L(M) \neq \emptyset$ because $x \notin E_{DFA}$  
					- This must mean there is a path from the start to accept state for some string $w$ for $M$. Thus, $M_{2}$ will reject and $x \notin L(M_{2})$
			2. $E_{DFA} \subseteq L(M_{2})$
				- Means $x \in E_{DFA} \rightarrow x \in L(M_{2})$
				- Contrapositive: $x \notin L(M_{2}) \rightarrow x \notin E_{DFA}$
				- Assume $x \notin L(M_{2})$
				- Case 1: $M_{2}$ found $x$ is not an encoding such that x is a DFA
					- $x \notin E_{DFA}$ by definition
				- Case 2: There exists a path for $M$ where $x = <M>$ between $M$'s start state and accept state
					- Consider the string y that is equal to the sequence of characters on transitions along the path. Then when you run M on y it accepts. Therefore $L(M) \neq \emptyset$
			3. M is a decider
				- Prove this by going through all of M's steps
					- Type checking halts
					- Running BFS on M halts
					- Therefore M always halts and is a decider
- $E_{DFA}$ is also recognizable since it is decidable
- $EQ_{DFA}$ is decidable and recognizable since it's decidable
	- Symmetric Difference Theorem: $X = Y \iff (X \cap \bar{Y}) \cup (Y \cap \bar{X}) = \emptyset$
		- Intuition: If X and Y are the same then if you inverse X and you intersect it with Y than they shouldn't cross over at all
	- Construction
		- Create a new DFA that recognizes the symmetric difference of $L(X)$ and $L(Y)$ and check if it's empty
			- Checking empty: (in $E_{DFA}$, we have a decider for this proved previously for this)
			- All construction operations are will halt because DFA is finite
- $A_{NFA}, E_{NFA}, EQ_{NFA}$ are also all decidable because they can use the subset construction ([[Simulating NFA with DFA]]) to be converted to DFAs and we can run the deciders for $A_{DFA}, E_{DFA}, EQ_{DFA}$

## Decidability and Recognizable Theorem
**- Theorem: A language is decidable iff it and its complement are both recognizable**
- Proof: 
	- Suppose $A$ is decidable. Then consider the decider $M$ where $L(M) = A$. Build $M'$ from $M$ by swapping accept and reject states. Then $L(M') = \bar{A}$. 
	- Suppose A is recognizable and $\bar{A}$ is recognizable. Build a decider for A.
		- M = "on input w:
			- type check
			- Let R be a recognizer for A for and $R'$ be a recognizer for $\bar{A}$
			- simulate R and simulate $\bar{R}$ on w
			- for i = 1,2,3,....
				- run R and R' on w for i steps
			- if  accepts than accept, if $\bar{A}$ accepts then reject"
- Therefore the complement of $A_{TM}$ is unrecognizable.
- $\bar{A_{TM}}$ is [[Co-Recognizable Languages]]
- 