## Claim
- If $A$ is a language that can be recognized by a DFA then $\overline{A}$ can also be recognized by a DFA.
- Equivalent to: "the class of languages that can be recognized by DFAs is closed under complementation"
## Proof
- Overview: 
	- Using general idea for [[Closure Proofs]]
	- Define 2 [[DFAs]] using the [[Formal 5-Tuple DFA Definition]], $M$ and $M'$
	-  Prove between $L(M') = \overline{A}$ using [[Set Equality Proof]]
- Proof:
1. Let $A$ be a language that can be recognized by a DFA $M = \left( Q, \Sigma, \delta, q_{0}, F \right)$ such that $L(M) = A$ (aka M ends on accept state for everything in A)
2. Define $M' = (Q, \Sigma, \delta, q_{0}, \overline{F})$
3. Claim of correctness: $M'$ recognizes $\overline{A}$
	- WTS $L(M') = \overline{A}$
	- Show $L(M') \subseteq \overline{A}$ and $\overline{A} \subseteq L(M')$
		- $\overline{A} \subseteq L(M')$
			- Suppose $x\in \overline{A}$. Then the computation of $M$ on x ends on a reject state. i.e. $\delta^*(q_{0}, x)\notin F$ 
			- So $\delta^*(q_{0}, x)\in \overline{F}$ 
			- Therefore the computation of $M'$ on x ends on a accept state of $M'$. Therefore $x\in L(M')$
			- In english: *M ends on a reject state for elements in A compliment, so M' must end on an accept state for elements in A compliment*
		- $L(M') \subseteq \overline{A}$
			- Suppose $x \in L(M')$ . This means that $\delta^*(q_{0}, x)\in \overline{F}$.
			- So $\delta^*(q_{0}, x) \notin F$. 
			- Therefore the computation of $M$ ends on a reject state of M. Since $A$ is the language that can be recognized by DFA M and $x$ is not recognized in DFA $M$, $x \in \overline{A}$ . This proves that elements in $L(M')$ must also be in $\overline{A}$ .