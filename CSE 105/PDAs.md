## Definition
- Formal Definition of PDA: [[Formal 6-Tuple PFA Definition]]
- If L is regular then there is a PDA that recognizes it
	- Suppose L is regular. Then there is a DFA M that recognizes L. Create a PDA from M by changing the delta function so that $\delta'(q,x,\epsilon) = \{ \delta(q,x), \epsilon \}$ which basically copies all the transitions from the DFA and gives them a $\epsilon \rightarrow \epsilon$ transition. 
- The languages recognized by PDAs is the set of [[Context Free Languages]]
- Non deterministic PDAs are kind of different and are not the focus of this class
- PDAs recognize more than an NFA or DFA and it isn't always possible to reconstruct a NFA or DFA from a PDA
- [[Closure]] under
	- [[Union]] (adding a spontaneous move from new state to start state), 
	- [[Concatenation]] (need to make sure the stack is empty first, then add spontaneous move from accept states from one machine to start of the other)
	- [[Kleene Star]] (add a fresh start state and spontaneous moves from the accept states to the old start state, need to empty stack)

## Designing a PDA given a Language
1. Understand L: Identify Strings in and not in L
2. Sketch a high level diagram that determines membership in L (think about what to be popping and pushing)
3. Translate to informal description of PDA
4. Translate to state diagram and/or formal definition of PDA
5. Confirm consistency with test cases
- Use # or $ to designate the bottom of the stack in the beginning if we need to push elements to count and pop elements to count to see if we have the same number of both![[Pasted image 20231107114206.png]]
- 
![[Pasted image 20231107113325.png]]

## Computation Tree Example
1. ![[Pasted image 20231107110705.png]]
2. ![[Pasted image 20231107110716.png]]