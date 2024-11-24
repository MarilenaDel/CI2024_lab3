# CI2024_lab3
In order to solve the n^2-1 puzzle problem I chose to implement an A* search algorithm using the Manhattan Distance as heuristic function.
This heuristic is admissable because it calculates the minumum possible distance by summing the moves needed for each tile to reach its goal position, so it never overestimates the cost. It is also consistent because the estimated cost associated with the current state is at most equal to the sum of the cost of the next state and the one needed to reach it.
The closed_set variable is keeping track of visited states and their costs, preventing loops during the search.

I kept the initial state random, obtaining it as a "scrumbled" version of the goal state, in order to avoid generating unsolvable configurations.
