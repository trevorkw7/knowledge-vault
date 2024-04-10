## Idea
- A language can be recognized by a DFA iff A can be recognized by an NFA
	- To show this we need to show that all languages recognized by DFA can be recognized by NFA (direction 1) and that all languages recognized by NFA can be recognized by DFA (direction 2)
	- Direction 1: 
		-
## Proof
- Overview:
-  To prove the *idea* we need to show that:
	- all languages recognized by DFA can be recognized by NFA (direction 1) 
	- and that all languages recognized by NFA can be recognized by DFA (direction 2)
- Direction 1: 
	- Given DFA $(Q, \Sigma, \delta, q_{0}, F)$ 
	- Build NFA $(Q, \Sigma, \delta ', q_{0}, F)$
	- With $\delta'$ defined as $\delta ' =$
		- $\{ \delta(q,x) \}$ if $x \in \Sigma$
		- $\emptyset$ if $x=\epsilon$
- Direction 2: 
	- Given A, a language recognized by an NFA $N = (Q, \Sigma, \delta, q_{0}, F)$ $L(N) = A$, want to show there is some DFA $M$ with $L(M) = A$ 
	- Construction: 
		- Idea: Track the possible states NFA might be in
		- $M = (P(Q), \Sigma, \delta', S, F')$
			- where $S$ is the set of all states we can be in within the NFA without consuming any input: $q_{o} \cup \delta^*((q_{0}, \epsilon))$ 
				- Here the delta star /  [[DFA Computation Function]] returns the set of states we can get to from the $q_{0}$ state using only the $\epsilon$ character
			- ![[Pasted image 20231027175938.png]]
			- where $F'$ is the set of all subsets $x \subseteq Q$ such that $F \cap x \neq \emptyset$

## Subset Reconstruction Example
1. ![[Pasted image 20231027183139.png
2. ![[Pasted image 20231027183224.png]]