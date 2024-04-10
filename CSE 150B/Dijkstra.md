#CSE150B 
- Small change to the data structure for the "frontier". We use a priority queue instead of a queue and pop the element with minimum cost each time.
- Is an "uninformed search", no data on where goal should be
- Usually we have some idea of where we want to go but Dijkstra makes no use of this information which is why [[A*]] is better

# Overview
## First round
- Frontier is initialized to starting node
- Pop starting node from frontier
- Push the neighbors of the node that was popped
## Intermediate / K Iteration
- Priority queue will help us choose the best / lowest cost node in the current frontier
- Pop the current node in the frontier
	- Check if we reached the goal, if yes we've found the shortest path to the goal
- There are 3 types of nodes we consider that are neighbors to the current node
	- Explored
		- Throw away
	- Unexplored
		- Add it to the frontier that we will form after this iteration
		- Add the cost of the current node + cost from current node to new node
	- In Frontier
		- Double check if the cost assigned to this node is now lower on our revisit of it. If it is, than we rewrite it.
## Why does it work?
- The goal check needs to in the pop step not the push step for the same reason why we need the double check, the initial time its added to the frontier may not be the shortest path to it.
- Need to make the argument that when we pop the node in the frontier, that is the shortest path to that node.
- Proved by the [[Separation Property]]
