Project Link：http://inst.eecs.berkeley.edu/~cs188/pacman/home.html

## **Finding a Fixed Food Dot using Search Algorithms** 

*Implement the depth-first search(DFS) algorithm*
```
python pacman.py -l tinyMaze -p SearchAgent
python pacman.py -l mediumMaze -p SearchAgent
python pacman.py -l bigMaze -z .5 -p SearchAgent
```
*Implement the  breadth-first search(BFS) algorithm*
```
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5
```
*A\* search*
```
python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic 
``` 
## **Finding All the Corners** <br />
*BFS*
```
python pacman.py -l tinyCorners -p SearchAgent -a fn=bfs,prob=CornersProblem
python pacman.py -l mediumCorners -p SearchAgent -a fn=bfs,prob=CornersProblem
```
*DFS*
```
python pacman.py -l tinyCorners -p SearchAgent -a fn=dfs,prob=CornersProblem
python pacman.py -l mediumCorners -p SearchAgent -a fn=dfs,prob=CornersProblem
```
*Implement a heuristic for the CornersProblem in cornersHeuristic*
```
python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5
``` 
