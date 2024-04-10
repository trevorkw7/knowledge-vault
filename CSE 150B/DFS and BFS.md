## Comparison
- DFS uses a stack
	- Stack is the "frontier", keeps track of nodes that have been visited but not fully explored
	- LIFO so when we hit a dead end we mark the current node as explored by popping the top off and back track to the previous node and explore, continue until we find goal node
- BFS uses a queue
	- Queue stores all nodes that have been discovered (immediately adjacent to visited node).
- This changes the order of exploration
## New Terminology 
- Frontier
	- A container with the nodes that we're currently considering
	- Start with only the initial state in the frontier
## Why enumerate nodes?
- Because we care about the order we took to get to the goal state, we're enumerating the path that we take
- Not enough to just find where the goal state is