## Proof
- To prove a [[Language]] is regular you must be able to do one of the following
	- Build a DFA whose language is this set
	- Build an NFA whose language is this set
	- Build a [[Regular Expressions]] describing this set
	- Use [[Closure]] properties of the class of regular languages to construct this set from others known to be regular
	- Language is finite because any finite language is regular
		- Can just union everything in that language together
- To prove that a language is not regular
	- Show that there is some string that is should be pumpable but isn't
## Properties
- There are countably infinitely many regular languages 
	- Because every regular language can be described by a regular expression and each regular expression is over an alphabet: ![[Pasted image 20231027194308.png]]
	- The set of strings over an alphabet is countably infinite under [[Counting Languages]]
	- Thus, there are countably infinitely many regular languages
- By [[Counting Languages]], since regular languages are countably infinite and all languages is uncountably infinite
	- $\{ \text{Regular Languages} \} \subset\neq \{ \text{All Languages} \}$
	- Thus non regular languages exist
	- If we know some languages are non-regular, we can conclude others must be too using the [[Closure Proofs]] of regular languages