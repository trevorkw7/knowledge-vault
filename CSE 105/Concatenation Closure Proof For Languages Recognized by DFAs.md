## Claim
 - If $A$ and $B$ are languages that can be recognized by DFAs then $A \circ B$ can also be recognized by DFAs.
- Equivalent to: "the class of languages that can be recognized by DFAs is closed under the **concatenation operation**"
## Proof
- Naive solution:
	- If we know the language is built from concatenating one string that can be recognized by DFA $M_{1}$ and another another string recognized by $M_{2}$, we can just make a DFA that runs the string in $M_{1}$ and then jump to $M_{2}$ 
	- Problem: How do we know when to jump? Can't just jump when we reach accept state because it could jump prematurely
- Solution: [[Nondeterminism]]
	- We take all the accept states from $M_{1}$ and make  [[Spontaneous Transitions]] to the start state of $M_{2}$ 
	- "Against the rules" in a DFA but NFAs can be converted back to DFAs
	- Given $M_{1} = \left( Q_{1}, \Sigma, \delta_{1}, q_{1}, F_{1} \right)$ and $M_{2} = (Q_{2},\Sigma, \delta_{2},q_{2},F_{2})$ build my NFA $N$ where $N=\left( Q_{1} \cup Q_{2}, \Sigma, \delta , q_{1}, F_{2}\right)$
		- Union our states
		- Same alphabet
		- New start state is the start state of $M_{1}$ which is $q_{1}$ 
		- New accept states are the accept states from $M_{2}$ which is $F_{2}$ 
		- Delta function becomes the following:
			- ![[Pasted image 20231026145924.png]]
			- Purple is copying the transitions from $M_{1}$ 
			- Green is copying the transitions from $M_{2}$
			- Red is creating the new transitions from the accept states of $M_{1}$ to the start state of $M_{2}$ .
## How to build [[NFA]] that recognizes concatenation 
- Connect all accept states for one DFA with [[Empty String]] transitions to the start state of the second DFA
## Building NFA Example
1. ![[Pasted image 20231025013002.png]]
2. ![[Pasted image 20231026143220.png]]![[Pasted image 20231026143227.png]]