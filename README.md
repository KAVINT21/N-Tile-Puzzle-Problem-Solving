# N-Tile-Puzzle-Problem-Solving
Given problem is a programming and making report. The problem is based on forward search engine that supports multiple search strategies and uses this implementation to findSolving N-Tile problem using tree-based search algorithms which include BREATH FIRST, DEPTH FIRST, BEST FIRST SEARCH, A* Search, and Hill Climbing.


# Summary

Given problem is a programming and making report. The problem is based on forward search
engine that supports multiple search strategies and uses this implementation to find solutions for a
solving N tile puzzle problem. You need to implement tree-based search algorithms which include
BREATH FIRST, DEPTH FIRST, BEST FIRST SEARCH, A* Search, and Hill Climbing. Next
step is to create a report based on the search implementation to solve the puzzle.

# Implementation

You can implement the programming using either C/ Python for problem 1. You must gain
permission before using anything else. Assignment work will be tested on a standard Microsoft
Windows XP operating system.

# Search Algorithms

PROBLEM – SOLVING N TILE PUZZLE PROBLEM
You are given a row containing 2N tiles arranged in 2N + 1 spaces. There are N Red tiles (R),
N Green tiles (G), and a single empty space. The tiles are initially in an arbitrary ordering.
Your goal is to arrange the tiles such that all green tiles are positioned to the left of the red
ones, and one red tile is in the rightmost position. The goal position of the empty space is not
specified. Tiles can be moved to the empty space when the empty space is at most N cells
away. Hence there are at most 2N legal moves from each state. The cost of each move is the
distance between the tile and the empty space to which it moves (1 to N). “Circular” moves
(i.e. moves wrapping from one side of the row to the other) are not permitted.
To illustrate the tile domain, consider the trivial case where N = 2.
Initial state may look like:

G R - R G
There are 4 successors to the initial state:
G R - R G
G R R - G
G R G R -
- R G R G

There are 4 goal states:

G G R - R
G G - R R
G - G R R
- G G R R

# IMPLEMENTATION PROCEDURE

• Your implementation should read in an arbitrary starting state for tile problems containing up
to 21 positions (10 RED, 10 GREEN, and 1 space). Each input file contains a single line
specifying the initial state using R to represent a RED tile, G to represent GREEN, and x to
represent the space. For example, one possible starting state for a 7-position problem is the
string:
GRRGXGR
You should use one operator, move x, to specify which tile to move into the current empty
position. x is the position of the card (starting from left to right). Note that you only need
specify which card to move since it will always move into the single empty position. In the
absence of any other heuristic function that determines which tile to move, all legal moves
should be considered in increasing order (i.e. from 0 to 2N + 1; move 1 occurs before move
3).
• Implement the solutions to solve the puzzle using:
1) BREATH FIRST SEARCH TREE
2) DEPTH FIRST SEARCH TREE.
3) BEST FIRST SEARCH
4) A * SEARCH
5) HILL CLIMBING

# PROGRAMMING INSTRUCTIONS

In this programming, you will have to make decisions about how to solve puzzle problems, states,
nodes, etc. You need to implement the following search algorithms:
Search Type Description Method
Depth-first search Select one option, try it, go back when there are
no more options

# DFS

Breadth-first search Expand all options one level at a time BFS
Best-first (F=g+h) Take the best (weighted score), okay to go back BEST
A* SEARCH Priority queue sorted according to the heuristic
function

# A* SEARCH

Hill climbing( Using
H function only)
Take the best (weighted score), no going back HC


# OUTPUT:

# Initial Display for selecting the algorithm:

![image](https://github.com/KAVINT21/N-Tile-Puzzle-Problem-Solving/assets/95117554/c8a084d4-31ba-4db3-8956-ae0dd0ab5744)

 
# Selecting BFS and entering the state:

![image](https://github.com/KAVINT21/N-Tile-Puzzle-Problem-Solving/assets/95117554/fad3cee1-7bb7-49f6-892b-8c700b1dc0bd)


# Selecting BFS and choosing 10 Tiles as input:
 
![image](https://github.com/KAVINT21/N-Tile-Puzzle-Problem-Solving/assets/95117554/bb368db3-21f8-4460-b453-35824696ebf2)

![image](https://github.com/KAVINT21/N-Tile-Puzzle-Problem-Solving/assets/95117554/cf0a4e6c-7f52-4da8-aad0-c029fa6aa9cf)


# Selecting DFS and input 4 Tiles as input:

![image](https://github.com/KAVINT21/N-Tile-Puzzle-Problem-Solving/assets/95117554/bd852f54-27ff-40c5-9d91-0db568b01267)


# Selecting Best First search and input 4 Tiles:

![image](https://github.com/KAVINT21/N-Tile-Puzzle-Problem-Solving/assets/95117554/85ea1632-5d9b-40d4-af25-45a78d6ae4c5)


# Selecting A Star Search and input 6 Tiles:

 ![image](https://github.com/KAVINT21/N-Tile-Puzzle-Problem-Solving/assets/95117554/cc8e8a37-66fc-4ed1-bc65-791107d72403)


# Selecting Hill climbing and input 4 Tiles:

 ![image](https://github.com/KAVINT21/N-Tile-Puzzle-Problem-Solving/assets/95117554/3a40a998-1bff-4f5a-9f2f-85ae9349528a)

 ![image](https://github.com/KAVINT21/N-Tile-Puzzle-Problem-Solving/assets/95117554/48c6cf4d-213f-4b48-a32e-accb481c1f87)


# Giving Goal State as Input:

![image](https://github.com/KAVINT21/N-Tile-Puzzle-Problem-Solving/assets/95117554/24b4d9b8-0dbf-42bd-8e3b-2108e69faeec)
