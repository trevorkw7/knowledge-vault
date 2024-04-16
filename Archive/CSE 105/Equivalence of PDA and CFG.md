## Proof
- Claim: If $L$ is described by a CFG ([[Context Free Grammar]])then there exists a PDA that recognizes $L$
- Proof Idea:
	- Example: $G=(\{ S,T \}, \{ 0,1 \}, R, S)$
	- $R = S \rightarrow 0S{1} | 1T | 1$
	- $T \rightarrow 1T | 1$
	- 