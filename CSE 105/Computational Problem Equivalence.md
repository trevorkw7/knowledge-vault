## Computational Problem Equivalence
- $A_{REX} \neq A_{NFA} \neq A_{DFA}$ even though they recognize the same languages and their difficulty level are the same but their encoding types are different 
	- Ex: $A_{REX} = \{ <R,w> \mid \text{R is a regex and } w\in R \}$
	- vs $A_{DFA} = \{ <M,w> \mid \text{M is a DFA and } w \in M \}$