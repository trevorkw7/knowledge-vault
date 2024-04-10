## Claim
- If $A$ and $B$ are languages that can be recognized by DFAs then $A\cap B$ can also be recognized by DFAs
- Equivalent to: "the class of languages that can be recognized by DFAs is closed under the **intersection** operation"
## Proof
- Two ways to prove:
	- Construction: almost identical to [[Union Closure Proof For Languages Recognized by DFAs]], except the accept states are only the ones that are in BOTH $F_{1}$ and $F_{2}$ 
	- Proof using Complement and Union Closure:
		- Suppose $A$ and $B$ are recognized by DFAs. 
		- Then $\overline{A}$ and $\overline{B}$ can be recognized by DFAs 
			- (by [[Complementation Closure Proof For Languages Recognized by DFAs]]). 
		- Then $\overline{A} \cup \overline{B}$ can be recognized by DFAs 
			- [[Union Closure Proof For Languages Recognized by DFAs]]
		- Then $\overline{\overline{A} \cup \overline{B}} = A \cap B$ can be recognized by DFAs! 
		- Visual Proof:![[Pasted image 20231024213315.png]]