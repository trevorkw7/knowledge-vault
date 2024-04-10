### Related
- [[NFA Computation Examples]]
- [[DFAs]]
## Definition
- [[Nondeterminism]]
- Nondeterministic finite automata
- Allows for several or zero alternative computations on the same input
	- $\delta(q, x)$ may specify more than one possible next state
	- $\epsilon$ transitions / [[Spontaneous Transitions]] allow the machine to transition spontaneously without consuming any input symbols
- Formal Definition of NFA: [[Formal 5-Tuple NFA Definition]]
- Rules:
	- $\delta: Q\times \Sigma_\epsilon \rightarrow P(Q)$
		- $\Sigma_{\epsilon} = \Sigma \cup \{ \epsilon \}$
		- Means that our transition function has a transition at every state Q for every character in our alphabet *including the empty string* to any combination of states in Q (power set).
## Characteristics
- Only requires one possible computation to end in accept state for a string to be recognized
-  Swapping accept and non accept states won't recognize compliment language (unlike [[DFAs]])
