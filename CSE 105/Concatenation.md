### Related: [[Concatenation Closure Proof For Languages Recognized by DFAs]]
## Definition
- A language specific set operation
- "$r_{1} \circ r_{2}$ is the language that includes any string from $r_{1}$ concatenated with any string from $r_{2}$"
	$$
r_{1} \circ r_{2} = \left\{ w_{1} \circ w_{2} \mid w_{1} \in r_{1} \wedge w_{2} \in r_{2} \right\} 
$$


## Notation
- The operator is denoted with $\circ$ but is often omitted so when we see empty space between [[Language]]s we assume that they are concatenated
$$
## Example 
1. Which of these strings are NOT in the language $\left\{ 0, 00, 11 \right\} \circ \left\{ 0, 10, 101 \right\}$ ?
		A. 00101
		B. 11010
		C. 000
		D. 1110
			Answer: B 
2. What is $\left\{ ab, ba, a \right\} \circ \left\{ bb, b, \epsilon \right\}$? How many elements are there there?
3. 
		= $\left\{ ab, ba, a, abbb, abb, babb, bab, abb, ab \right\}$
		Duplicates: abb, ab, 
		= $\left\{ ab, ba, a, abbb, abb, babb, bab \right\}$
		Elements: 7

