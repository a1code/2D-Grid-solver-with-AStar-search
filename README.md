# 2D-Grid-solver-with-AStar-search

**Implementation Summary** :
- Wrote modules in Python for 2D grid generation and performing A* search on a grid.
- Implemented and visualized path planning between source and goal.
- Performed experiments and reported observations to compare the performances of different variations of the A* algorithm .  
  
  
**Abstract** :
An agent in a gridworld has to move from its current cell to the given cell of a non-moving target, where the gridworld is not fully known. They are discretizations of terrain into square cells that are either blocked or unblocked.  

The agent moves along a path that satisfies the following three properties:
1. It is a path from the current cell of the agent to the target.  
2. It is a path that the agent does not know to be blocked and thus assumes to be unblocked, i.e., a presumed unblocked path.
3. It is a shortest such path.

The agent repeatedly calls the A* search algorithm to find a "shortest presumed-unblocked path" from its current cell to the target. The cycle stops when the agent:  
• either reaches the target, or  
• determines that it cannot reach the target because there is no presumed-unblocked path from its current cell to the target, and it is thus separated from the target by blocked cells.

In the former case, the agent reports that it reached the target. In the latter case, it reports that it cannot reach the target.
