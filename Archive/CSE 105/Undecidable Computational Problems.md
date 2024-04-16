## Summary
$A_{TM}$ is recognizable but not decidable
$\bar{A_{TM}}$ is not recognizable because decidable languages are closed under complementation (see [[Decidable Languages]])
$\bar{A_{TM}}$ is not recognizable because if it was, then $A_{TM}$ would be decidable (see [[Decidable Languages]])

## The existence of undecidable TMs
- Need to prove that every single TM doesn't decide that problem
- NOT every problem is decidable because:
	- The set of all regular languages is countably infinite
	- The set of all languages is uncountably infinite
	- We can make a similar argument to show that not all computational problems are decidable
	- Proof:
		- The set of **Turing-recognizable languages is countable** because each Turing-recognizable language is associated with a TM, so **there can be no more Turing-recognizable languages than TMs**
		- We know that the **number of TMs is countably infinite** because they are represented by finite strings (like 0s and 1s)
		- Therefore: since $\text{Turing decidable languages} \subseteq \text{Turing recognizable languages}$ and Turing recognizable languages are countably infinite, then the set of **Turing decidable languages must be countably infinite**
		- Which means that **there are languages that aren't Turing decidable** since there are uncountably infinite languages

## We can't just simulate
- $A_{TM} = \{ <M,w> \mid \text{M is a TM and } w \in L(M) \}$
	- This is a set of all strings that encode TMs and strings
	- Define another Turing machine N in an *attempt* to decide $A_{TM}$ 
		- On input $<M,w>$:
			1. Simulate M on w
			2. If M accepts, accept. If M rejects, reject
		- N doesn't decide $A_{TM}$ because we could give it an encoding $<M,w>$ that isn't in $A_{TM}$ that causes it to never halt
		- N recognizes $A_{TM}$ because it will always accept if $w \in L(M)$
			- **$A_{TM}$ is recognizable**
	- This approach which mirrors what we did to build a dec
	- idea for $A_{DFA}$ doesn't work

## Nail in the coffin: [[Diagonalization Proof]]
