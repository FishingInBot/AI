# AI PRojects
These are my implementations for each of the AI programming assignments.

## Dijkstra's Shortest Path Algorithm
Suppose there is graph having nodes, where each node represents a city. A few pair of nodes are connected to each other, with their distance mentioned on the conneting edge, as shown in the figure below:<br>
<img style="float: center;height:250px;" src="/Dijkstra/graph1.png"><br>

To find the shortest path from a given source to destination node in the example above, a Greedy approach would be - *At each current node, keep track of the nearest neighbour. We can determine the path in the reverse order once we have a table of nearest neighbours (optimal previous nodes).* For example, C is the optimal previous node for E. This way, the shortest path from `A` to `E` would be `A --> D --> C --> E`, as shown below:<br>
<img style="float: center;height:250px;" src="/Dijkstra/graph2.png"><br>

And, if we wish to print the distance of each node from `A`, then it would look like:<br>
<img style="float: center;height:250px;" src="/Dijkstra/graph3.png"><br>

Here, the **Previous Optimal Node** is the "best" node which could lead us to the current node. 

### The Problem
Using Dijkstra's algorithm, find the shortest path to all the nodes starting from a given single source node.  You need to print the distance of each node from the given source node. For the example quoted above, the distance of each node from `A` would be printed as:<br>
```
{'A': 0, 'D': 2, 'B': 5, 'E': 4, 'C': 3, 'F': 6}
```

## Knight's Isolation
In this assignment, you will experiment with adversarial search techniques by building an agent to play knights Isolation. The players control tokens that move like chess queens, this version of Isolation gives each agent control over a single token that moves in L-shaped movements--like a knight in chess.
### Isolation
In the game Isolation, two players each control their own single token and alternate taking turns moving the token from one cell to another on a rectangular grid. Whenever a token occupies a cell, that cell becomes blocked for the remainder of the game. An open cell available for a token to move into is called a "liberty". The first player with no remaining liberties for their token loses the game, and their opponent is declared the winner.
In knights Isolation, tokens can move to any open cell that is rows-2 and column-1 or columns-2 and row-1 away from their current position on the board. On a blank board, this means that tokens have at most eight liberties surrounding their current location. Token movement is blocked at the edges of the board (the board does not wrap around the edges), however, tokens can "jump" blocked or occupied spaces (just like a knight in chess).
**Note:** my implementation is the CustomPlayer method. Theoretically, at some high depth two CustomPlayers will fill the board against eachother, though this will take some time.

## Pacman Project
This is my implementation of Berkeley's Pacman AI project, https://inst.eecs.berkeley.edu/~cs188/sp23/projects/. I have not implemented "Project 0".

### Project 1: Search
This implements several search algorithms to complete certain mazes based on different objectives.

### Project 2: Logic
In process...