## Claim
- If $A$ and $B$ are languages that can be recognized by DFAs then $A \cup B$ can also be recognized by DFAs.
- Equivalent to: "the class of languages that can be recognized by DFAs is closed under the **union operation**"
## Proof
- Overview: 
	- Show that we can build a DFA that recognizes $A_{1} \text{ and } A_{2}$
	- Strategy: build a DFA that recognizes $A_{1}$ and another DFA that recognizes $A_{2}$, then combine them to create a new DFA so that we only accept a string if *either or both* $A_{1}$ and $A_{2}$ accept.
	- "Run in Parallel"
- Proof: Let A1, A2 be any two languages over $\Sigma$ that can be recognized by DFAs
	- Given $M_{1} = (Q_{1}, \Sigma, \delta_{1}, q_{1}, F_{1})$ such that $L(M_{1}) = A_{1}$ and $M_{2} = $M_{1} = (Q_{1}, \Sigma, \delta_{2}, q_{2}, F_{2})$ 
	- WTS $A_{1} \cup A_{2}$ can be recognized by a DFA, aka $L(M) = A_{1} \cup A_{2}$
	- Define $M = (Q_{1} \times Q_{2}, \Sigma, \delta, (q_{1}, q_{2}), \{ (r,s) \in Q_{1} \times Q_{2} \mid r \in F_{1} \vee s\in F_{2} \})$ 
		- New states is cartesian product
		- Same alphabet
		- New delta function: $\delta ((r,s), x) = (\delta_{1}(r,x), \delta_{2}(s,x))$ for (r,s) in $Q_{1} \times Q_{2}$ and $x \in \Sigma$. Basically draw the transition functions for where each letter in the alphabet $\Sigma$ goes from each state and make a new state that has (state letter goes to in dfa 1, state letter goes to in dfa 2)
		- Start state is an ordered pair
		- New accept states is any ordered pair that contains a state from one of the F1 and F2 accept states.
- Proof with NFAs
	- Same as before but define NFA $N$ which recognizes $A_{1} \cup A_{2}$ as $N = (Q,\Sigma,\delta,q_{0},F)$ 
		- $Q = Q_{1} \cup Q_{2} \cup \{ q_{0} \}$ 
			- All states of $M_{1}$ $M_{2}$ and this new start state $q_{0}$ 
		- $\Sigma$ stays the same, same alphabet
		- $\delta = \delta(q,x) = \begin{cases} \delta_{1}(q,x) \text{ if } q \in Q_{1} \text{ and } x \in \Sigma \\ \delta_{2}(q,x) \text{ if } q \in Q_{2} \text{ and } x\in \Sigma  \\ \{ q_{1}, q_{2} \} \text{ if } q=q_{0} \text{ and } x = \epsilon \\ \text{null otherwise} \end{cases}$
			- Copy transitions from $M_{1}$ and $M_{2}$ and add new spontaneous transition that goes to both $q_{1}$ and $q_{2}$ when going from the start state
		- $q_{0} = q_{0}$
		- $F = F_{1} \cup F_{2}$
	- Note: Only works if $\Sigma$ is the same, $F_{1} \subseteq Q_{1}, F_{2} \subseteq Q_{}$

## How to build DFA that recognizes union of 2 DFAs
- There will most likely be states that are not reachable but if we start from the start states on each DFA and keep connecting ordered pairs till every state has an edge for each symbol in $\Sigma$, we've listed all reachable states and the transitions for those states!

## How to build a NFA that recognizes the union of 2 DFAs
- Create a new start state $Q_{new}$ and create spontaneous transitions between that and $M_{1}$ and $M_{2}$ ![[Pasted image 20231026150627.png]]
- If we can reach an accept state on either $M_{1}$ or $M_{2}$ that language is in the union!!
## Example
1. ![[Pasted image 20231023011233.png]]
2. ![[Pasted image 20231024210934.png]]



![[Pasted image 20231107131054.png]]
