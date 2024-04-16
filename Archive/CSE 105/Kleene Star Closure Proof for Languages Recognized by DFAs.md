## How to build a NFA that recognizes the Kleene Star of the Language over a DFA
- Create new accepting start state $q_{n}$ to FORCE recognize empty string with a spontaneous transition to the original start state
- Create new spontaneous transitions from all the accept states back to the original start state![[Pasted image 20231026152246.png]]
- Formal Definition of the constructed NFA:
- Given $M_{1} = \left( Q_{1}, \Sigma, \delta_{1}, q_{1}, F_{1} \right)$ build my NFA $N$ where $N=\left( Q_{1} \cup \{ q_{n} \}, \Sigma_{\epsilon}, \delta , q_{n}, F_{1} \cup \{ q_{n} \} \}\right)$ accepts the Kleene star of the language over N
	- $\delta: Q \times \Sigma_{\epsilon} \rightarrow P(Q)$ 
		- if $\delta((q,x))$ where $q \in Q_{1},x\in\Sigma$ use $\delta_{1}((q,x))$
			- Keep original states 
		- if $\delta((q,x))$ where $q \in \{ F_{1} \} \cup \{ q_{n} \},x = \epsilon$ go to $\{ q_{1} \}$
			- Add transitions from accept states back to start state (including the new start state)