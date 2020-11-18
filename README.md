https://github.com/elysio2/comp472-a2

# comp472-a2

This is a jupyter notebook project, using python 3, not requiring any additional modules except those included in python (queue, time, random, collections).

Heuristics: 

No heuristic takes into account the placement of 0, since it is pointless, because there will always be at least 2 misplaced tiles but never 1. 

h1 : Modified Hamming Distance. Each correct tile decreased the heurisitc by 2/3, since the sliding move creates a shortcut where a 3-cost move would only cost 2. For each valid goal state, the heuristic is computed, then the lowest of the 2 is returned.

h2: Modified Manhattan Distance. For each goal state, each tile's distance to its correct place is computed, up to a max of 2, since a tile 3 tiles from its correct placement might only cost 2 to move there.  