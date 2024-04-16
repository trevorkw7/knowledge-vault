### Related: [[Language Operations]]
## Definition
- Is a directed graph *wow like CSE 101, one way arrows from vertices to other vertices*
- Vocab:
	- States: vertices of this graph
	- Transitions: edges of this graph labeled with characters from [[Alphabet]] $\Sigma$
- Rules:
	- Every state has one outgoing transition for each character in $\Sigma$ 
		- Formally: $Q \times \Sigma \rightarrow Q$, differentiates DFA from [[NFAs]]
	- Only and exactly one vertex is labeled as start state
	- Each vertex is either a accept state or not
- [[Formal 5-Tuple DFA Definition]]
- 

## Input and Output
- Allowable input must be string over the alphabet of the transitions
- Output is binary, yes or no, accept or reject
	- ACCEPT: The computation ends in accept state (double circle)
	- REJECT: The computation ends in reject state (single circle)

## Computation
- The sequence of states that we go through in the DFA as we read in a input
- Formalized in [[DFA Computation Function ]]
- Has a unique computation path for every input


## Language Recognized by a DFA
- The set of strings it accepts
- Denoted by $L(M)$ where $M$ is the DFA

## Visuals
- Arrow points to the start state
- Alphabet is all the distinct characters labeling the edges
- Accept states have **double circles** 
- Transitions are shown via the arrows aka edges![[Pasted image 20231021024727.png]]


## DFA Building Tips
- To make the [[Empty String]] accepted, the first state must be an accept state
	- Just from observing this we can show that two machines recognize different languages if one has first accept state and the other doesn't
- The "trap state" is useful for avoiding a particular patern if we don't make it accept, if we make it accept then its useful for finding a patern
- Design and pick states with specific roles / tasks in mind
	- "Have not seen any of desired pattern yet"
	- "Trap state"
- If we need a memory for something like "how many As have we seen so far" we need a state for each distinct memory like "seen 1 A", "seen 2 As" 
- Can use the [[Closure Proofs]] to build DFAs for languages where "and", "nor", "or" is used. 


# Examples
[[Observing DFA Examples]]
[[Building DFA Examples]]