# MazeSolver-AI-Programming
Search algorithms (BFS, DFS, UCS, A* Search) for solving problem

- You can only go left, right, below or up. There is no option for diagonal moving
- Define maze as 2D list. For example:
```Python
mazeGraph = [
        ["-", 0, 1, 0, 1],
        ["-", "-", 2, 1, 2],
        [2, "-", 3, 0, "-"],
        [0, 2, 1, 1, "-"],
        [1, 0, 3, 1, "-"]
    ]
```
- "-" represent the wall, that's means can not pass on it.
- Each tile action cost is 1. And there are extra cost action on the tiles. 
  - For example: moving from (0,3) to (1,3) cost is 1, if we don't care about extra action cost, or
  - moving from (0,2) to (1,2) cost is (1 + 1) 2, if we care about extra action cost 
- Then start the program: (find a path between (0,0) to (4,2) with admissible a* search and without admissible a* search)

```Python
 mazeSolver = MazeSolverWithAStarSearch(mazeGraph, (0, 0), (4, 2))
 mazeSolver.astarSearchWithAdmissible()
 mazeSolver.astarSearchWithoutAdmissible()
```

- [Go to BFS Search](https://github.com/mehmetozanguven/MazeSolver-AI-Programming/blob/master/MazeSolverWithBFS.py)
- [Go to DFS Search](https://github.com/mehmetozanguven/MazeSolver-AI-Programming/blob/master/MazeSolverWithDFS.py)
- [Go to UCS Search](https://github.com/mehmetozanguven/MazeSolver-AI-Programming/blob/master/MazeSolverWithUniformCostSearch.py)
- [Go to A* Search](https://github.com/mehmetozanguven/MazeSolver-AI-Programming/blob/master/MazeSolverWithAStarSearch.py)
