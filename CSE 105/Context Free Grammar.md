## Definition
- Informally a collection of rules used to create a string
- CFGs generate languages
- Equally expressive as PDAs
	- We prove this with [[Equivalence of PDA and CFG]]
- Defined with the 4 tuple: $(V, \Sigma, R, S)$
	- V: Variables: finite set of (usually uppercase) variables V
	- $\Sigma$: Terminals: finite set of alphabet symbols $\Sigma$ (usually lower case)
		- Note: Terminals and Variables must be disjoint to avoid confusion
	- R: Rules/Productions: finite set of allowed transformations 
		- Always start with single variable, arrow to string of either your character alphabet or variable alphabet
		- ![[Pasted image 20231107121427.png]]
	- S: Start Variable
- There are many ways to build a CFG that recognizes the same language

## Convention
- capital letters are variables
- lowercase letters are characters

## Notation
- Derivation: a sequence of rule applications
	- "sequence of derivations where we can start at S and end at w": $S \rightarrow ^*W$

## Designing a CFG
- ![[Pasted image 20231107122506.png]]


## Closure under union
![[Pasted image 20231107122631.png]]

## Closure under concatenation
![[Pasted image 20231107122702.png]]
- "build two strings as you go"

## Closure under kleene star
![[Pasted image 20231107122825.png]]
- Can restart as many times as we want
## Examples
- Building a CFG that can recognize a non-regular language
- ![[Pasted image 20231107122315.png]]



## Facts
![[Pasted image 20231107123043.png]]
![[Pasted image 20231107123106.png]]