## Definition
- "$S^*$ is the set of all strings (finite) made up of any concatenations of strings within $S$"
- Formal Definition
$$
S^* = \{W_{1} \circ W_{2} \dots \circ W_{n} \mid W_1, W_{2}, \dots, W_{n} \in S \wedge n \geq 0 \}
$$

- Includes all of the strings as they are
- Always includes the empty string $\epsilon$
	- Result of concatenating your strings 0 times
- Infinite strings are not allowed

## Example
1. Which of these strings is NOT in the language $\left\{ a, bb, ca \right\}^*$
		A. aabbcaca
		B. caabbbb
		C. bbbbcabb 
		D. acabbbab
			Answer: D
2. Write out 10 elements of $\left\{ aa, ab, ba, a \right\}$
		Answer: $\left\{ aa, ab, ba, a, \epsilon, aaab, abba, baaa, aaaba, baab \right\}$
