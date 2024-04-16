## Technique
- Create an arbitrary DFA that can recognize [[Language]] $A$, take apart that DFA, and make a new DFA out of its parts that can recognize $A'$ , which is the language that has had a [[Language Operations]] done to it
- General strategy:![[Pasted image 20231024214228.png]]**

## Application to [[Language Operations]]
- [[Intersection Closure Proof For Languages Recognized by DFAs]]
- [[Complementation Closure Proof For Languages Recognized by DFAs]]
- [[Regular Operations]]:
	- [[Union Closure Proof For Languages Recognized by DFAs]]
	- [[Concatenation Closure Proof For Languages Recognized by DFAs]]
	- [[Kleene Star Closure Proof for Languages Recognized by DFAs]]
	- [[Union Closure Proof For Languages Recognized by PDAs]]
	- [[Concatenation Closure Proof For Languages Recognized by PDAs]]
	- [[Kleene Star Closure Proof for Languages Recognized by PDAs]]
- Can be used to prove something is a [[Irregular Language]] because the compliment of a non-regular language is non-regular 