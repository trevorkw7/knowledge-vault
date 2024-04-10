$(Q, \Sigma, \Gamma, \delta, q_{0}, F)$
	- Q is finite set of states
	- $\Sigma$ input alphabet
	- $\Gamma$ is the stack alphabet (doesn't have to be same as input)
	- $\delta: Q \times \Sigma_{\epsilon} \times \Gamma_{\epsilon} \rightarrow P(Q)$ is the transition function (described by table)
	- $q_{0} \in Q$ is the start state
	- $F \subset Q$ is the set of accept states 
- Epsilon $\epsilon$ is never part of the alphabet
## Example
![[Pasted image 20231107112049.png]]