## Mapping Reductions

![[Pasted image 20231214150535.png]]
![[Pasted image 20231214152850.png]]

- Given $A \leq_{m} B$ (i.e. A computable function $F$ exists that reduces A to B)
- Prove that the properties above in A must be in B (if A is hard, B must be at least as hard): 
	- Proof by contradiction by assuming B is solvable (decides, recognizes, etc.) to construct a machine $M$ that uses $F$ to take inputs of $A$ and converts them to $B$. This shows that A is also solvable which contradicts.



- Prove that properties above in B must be in A (if B is easy/solvable, A must also be solvable):
	- Create a machine that solves (decides, recognizes, etc.) A by reducing A to B and solving the B problem
![[Pasted image 20231214161855.png]]
![[Pasted image 20231214162455.png]]

- This makes conclusions about co-recognizable symmetric to recognizable when mapping A to B
	- "Co-recognizable easier than un-co-recognizable"

![[Pasted image 20231214175413.png]]
![[Pasted image 20231214175455.png]]
## Rice's Theorem + Time Complexity
![[Pasted image 20231214181756.png]]
- Informally: Rice's Theorem says any language about a non trivial language of Turing machines like $A_{TM}, E_{TM}, EQ_{TM}$ etc is undecidable.
- ![[Pasted image 20231214191756.png]]

## Polynomial-Time Mapping Reductions:
![[Pasted image 20231214192206.png]]
## P/NP
-  𝑃  = {𝐿 | 𝐿  can be decided in polynomial time by a deterministic Turing machine}
-  𝑁𝑃  = {𝐿 | 𝐿  can be decided in polynomial time by a nondeterministic Turing machine}
- NP Complete: Every language in NP is polynomial time reducible to languages in NP Complete
	- To show X is NP complete, show that a known to be complete NP problem reduces to X
- NP-Hard: All problems in NP can be polynomial time reduced to this. Not necessarily in NP.
	- NP-Complete $\subseteq$ NP
	- NP-Hard $\nsubseteq$ NP
	- NP $\cap$ NP-Hard = NP-Complete

$P \subseteq NP$
- ![[Pasted image 20231214201716.png]]
- NP Problems can be defined in 2 equivalent ways:
	- there exists a polynomial time NTM that decides A
	- solutions can be verified by a deterministic TM in polynomial time (there exists a V for A)
	- one of these implies the other
- Showing that a problem is in NP using the Verifier definition:
- ![[Pasted image 20231214203708.png]]
- Not known if NP is closed under complementation because it's not easy to verify that there a graph has no hamiltonian paths
- co-NP: means that complement is in NP
- If A in P, A complement also in P
- ![[Pasted image 20231214204627.png]]
- 
- Problems in NP: Any problem in P, NP Complete: NP Complete: SAT, 3SAT, CLIQUE (Finding a complete subgraph), HAMPATH (path through all vertices exactly once), TSP, KNAPSACK, 3 Coloring (Color a graph with 3 colors, no 2 adjacent verticies same color)
- $HALT_{TM}$ is NP-Hard:
- ![[Pasted image 20231214213126.png]]
![[Pasted image 20231214205551.png]]
![[Pasted image 20231214210655.png]]
- 3 SAT format is an AND of ORs (a or b or c) and (d or e or f)
- ![[Pasted image 20231214212150.png]]
  ![[Pasted image 20231214212724.png]]