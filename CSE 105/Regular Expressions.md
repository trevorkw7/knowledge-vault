## Definition
- Syntax used to describe [[Language]]s, not a language itself
- Assumption in this class is that the regex is over a described [[Alphabet]] $\Sigma$
- Symbols are used in conjunction with [[Language Operations]]: $\cup, \circ, *$,  and parentheses () to group 
- We apply the $L()$ function around this regular expression to describe the set that the symbol describes, means *the language of this regular expression*
- Itself is a string with an alphabet of the following allowable symbols: $\{ (,),\cup,\circ,*,\epsilon, \emptyset \} \cup \Sigma$
	- Where $\Sigma$ is the alphabet of the language we're trying to describe
	- The $\cup, \circ,*$ are [[Regular Operations]]
- Uses parenthesis () unlike sets which use curly braces {}

## Symbols to use: $\emptyset, \epsilon, 0, 1$
- Empty Set: $\emptyset$ means $\emptyset$
- **Set containing the empty string: $\epsilon$ means $\{ \epsilon \}$**
	- *This is not the same as just the empty string*
- Set containing 0: $\{ 0 \}$
- Set containing 1: $\{ 0 \}$

## Order of Operations
1. Apply star
2. Apply concatenation
3. Apply union

# How to build regular expressions
- Assuming the regular expression is over the language $\Sigma$
- Recursively defined by the following rules
- 1-3 are our "base elements" that we can stick together with $\cup$ and $\circ$ and use [[Kleene Star]]
1. $R = a$ where $a \in \Sigma$
2. $R = \emptyset$
3. $R = \epsilon$
4. $R = \left( R_{1} \cup R_{2} \right)$, where $R_{1}$ and $R_{2}$ themselves are regular expressions
5. $R = \left( R_{1} \circ R_{2} \right)$, where $R_{1}$ and $R_{2}$ themselves are regular expressions
6. $R_{1}^*$ where $R_{1}$ itself is a regular expression


## Example
1. Write the following as regular expressions
	- $\{ a,b,c \}$
		- $\{ a \} \cup \{ b \}, \cup, \{ c \}$
	- $\{ a^n \mid n \geq 0 \}$
		- has to include empty string and all concatenations above it
		- $= L(a^*)$
		- 
	- $\{ a^n | n \geq 1 \}$
		- has to include all concatenations of a except the empty string
		-  $L(aa^*)$ - this eliminates the empty string by concatenating it 
	- $\{ a, ab, abb, abbb, b, bb, bbb \}$
		- $(a \cup b \cup bb) \circ (\epsilon \cup b \cup bb)$ 
2. Let $A = \{ 1,01,001,\dots \}$, then say $0^*1$ is a regular expression that *describes* A 
	- (does not mean the are equal, must use )
3. $\{ 0 \}^* \circ \{ 1 \} = A$, T or F
	- True because these are sets and set operations which naturally equals A which is a language which is a set
4. Let $B = L(00^*1)$ and $C = L((00)^*1)$
	- B has 01 but C doesn't have 01 in the set therefore they are not equal
	- More formally, we can prove two sets are different if the element is in one set but not another
	- $01 \in B, 01 \notin C  \rightarrow B \neq C$ 
	- There are not subsets because B has elements C doesn't have and C has elements that B doesn't have
5. $\Sigma = \{ 0,1 \}$, $L((\Sigma \Sigma \Sigma \Sigma)^*) =\{  \}$
	- $=\{ \epsilon, 0000, 1111, 0101, 1010, 0001, 1000, 1100, 0011, 00000000, 11111111, \dots \}$
	- All binary strings with length a multiple of 4
6. Which of the following strings is **not** in the language described by $(((00)^*(11)) \cup 01)^*$?
	- Language of the inner set: $L((00)^*) =\{ \epsilon, 00, 0000, 000000, \dots \}$
	- Language of the inner set concatenated with 11 is $L((00)^*11) =\{ 11, 0011, 000011, 00000011, \dots \}$
	- Language of the inner set concatenated with 11 union 01 is: $L(((00)^*11) \cup 01) =\{ 01, 11, 0011, 000011, 00000011, \dots \}$
	- So this language can be any combination of these and the empty string
	- Choices:
	- A: 00
	- B: 01
	- C: 1101
	- D: $\epsilon$
		- Answer: A