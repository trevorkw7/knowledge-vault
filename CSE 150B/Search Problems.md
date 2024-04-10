#CSE150B 
# Components
- Initial States (Start)
- Goal States 
- Other elements in state space
- Actions
	- Takes you from one state to another state
	- Mappings from states to next states
- Cost or Reward
	- A metric for what is good and what is bad

# Solution
- Finding a sequence of actions that starts from the initial states and reaches the goals states

## Trees
- We can model search problems with a tree starting from an initial state and with each action branching into new possible states that we can go to
- Scalability is bad, for each layer / action made going down the tree, the number of possible states increases 
- This means that the there is no real solution because if the problem is big enough it becomes unsolvable
## AI
- All about solving NP complete and NP hard problems in ways that people didn't expect them to solve
## Intelligent Decisions
- About finding good paths in a gigantic tree of possible futures
# Examples
## 2048
- ![[Pasted image 20240409210322.png]]
- State: A pattern acceptable by the game
- Number of possible states / State spaces: 11 (can be 2,4,8,16,32,64,128,256,512,1024,2048) * 16 = 176
- Actions: 4 (up down left right)
## Robots
- Position the robot is currently in
- Actions: Controls sent to motors
- Size is infinite because continuous numbers  

# Types
[[DFS and BFS]]
[[Dijkstra]]
[[A*]]
