- Takes the start state and the word and outputs the state we ended up at
- Defined as $$
\delta^* (q,w) = \begin{cases}
q & \text{if } w = \epsilon \\ \\
\delta^*(\delta(q,a), w') & \text{if } w = aw'
\end{cases}

$$

- Where q is the state and w is the first word
- Recursively defined where base case returns the current state we're at if we're at the empty string and the recursive case returns the result of the *transition function $\delta$* function called with one less letter in the word
- Usage: when $\delta^*(q_{start}, w) \in F \text{(set of accept states)}$ the string is accepted by the DFA