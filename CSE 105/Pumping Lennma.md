## Definition
- Can be used to prove that a set is not regular
- Cannot be used to prove a set is regular
- Something is pumpable if we can split the string into xyz and we can cut out y or loop y any number of times and its still in in the language

## Proving that a set is not regular
- Assume that a set is regular, then it must pass the pumping lemma. Then show a set that fails the pumping lemma. You then have a contradiction which proves its not regular.

## Identifying non-regular languages
- Can't "count"
- Can only remember finitely far into past
- Can't backtrack
- Must make decisions in "real-time"

## Proof Template
- Proof: Consider an arbitrary positive integer p. WTS p is not a pumping length for L.
	- Find a string that 
	- 1. $\mid s\mid \geq p$
		- Length of the string is longer than the pumping length (number of loops we do)
	- 2. $s \in L$ 
		- String must be in the language L described
	- 3. No matter how we cut s into three viable pieces, some related string obtained by repeating the middle part falls out of L.
		- - $s=xyz$ with $\mid y\mid > 0$, $\mid xy\mid \leq p$
			- If we set one of the characters (say $A$) to p, then it must be composed of xy and maybe composed of z which we can break down into $s=xyz$ where $x = A^k$, $y=A^j$, and $z=A^r \text{remaining}^p$ so that $s=A^kA^jA^r\text{remaining}^p$.
			- We can change the number of times $y=A^j$ is repeated with $y^i  =A^{j *i}$ which will make $k+i*j+r$ bigger than p causing a mismatch between remaining and A.
## Proof Example
- Claim: The set $L=\{ 0^n 1^n \mid n \geq 0 \}$ is not regular
- - Proof: Consider an arbitrary positive integer p. WTS p is not a pumping length for L.
	- Find a string that 
	- 1. $\mid s\mid \geq p$
		- Length of the string is longer than the pumping length (number of loops we do)
		- In this case: $|s| = 2p$ 
	- 2. $s \in L$ 
		- String must be in the language L described
		- Yes, it has the $0^n 1^n$ form
	- 3. No matter how we cut s into three viable pieces, some related string obtained by repeating the middle part falls out of L.
		- $s=xyz$ with $\mid y\mid > 0$, $\mid xy\mid \leq p$
			- If we set one of the characters (say $A$) to p, then it must be composed of xy and maybe composed of z which we can break down into $s=xyz$ where $x = A^k$, $y=A^k$, and $z=A^r \text{remaining}^p$ so that $s=A^kA^kA^r\text{remaining}p$.
			- We can change the number of times $y=A^k$ is repeated 
		- In this case the string is 000000.... p times 111111... p times
		- Since 0 is repeated p times and $|xy| \leq p$ , we know x and y both have to be zeros so $x=0^k$ $y=0^m$ and $z=0^r 1^p$, where $k+m+r = p$.
		- Picking $i=0$, we go through the loop 0 times, which makes $s=xy^{0}z = xz = 0^{k+r}1^p$ which is not in L because $k+r < p$. Thus, no p can be a pumping length for L and L is not regular.
