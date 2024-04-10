## Definition
- A universal set operation
- Let $r_{1}$ and $r_{2}$ be languages over the [[Alphabet]] $\Sigma$ 
	- $$
r_{1} \cup r_{2} = \{w | w \in r_{1} \vee w\in r_{2}\}
$$
	- In english: r1 **union** r2 contains any string that is either in r1 or r2
		- *So contains anything in language 1, language 2, or both languages*
		- Related: [[OR]]
- Kind of like addition,  set union to the [[Empty Set]] is results in the original set

## Theorems
- [[Union Closure Proof For Languages Recognized by DFAs]]
## Example
1. What is $\left\{ aa, ab, ba, a \right\}\cup\ \left\{ bb,b,ba,\epsilon \right\}$? 
		= $\left\{ aa, ab, ba, a, bb, b, ba, \epsilon \right\}$
		= $\left\{ aa, ab, ba, a, bb, b, \epsilon  \right\}$
	- How many distinct elements are there [[Cardinality]]?
		- Answer : 7
		- *We only count ba in this case once*
	- Related: [[Empty String]]


