# N-Tile-Puzzle-Problem-Solving
Given problem is a programming and making report. The problem is based on forward search engine that supports multiple search strategies and uses this implementation to findSolving N-Tile problem using tree-based search algorithms which include BREATH FIRST, DEPTH FIRST, BEST FIRST SEARCH, A* Search, and Hill Climbing.


Summary

Given problem is a programming and making report. The problem is based on forward search
engine that supports multiple search strategies and uses this implementation to find solutions for a
solving N tile puzzle problem. You need to implement tree-based search algorithms which include
BREATH FIRST, DEPTH FIRST, BEST FIRST SEARCH, A* Search, and Hill Climbing. Next
step is to create a report based on the search implementation to solve the puzzle.

Implementation

You can implement the programming using either C/ Python for problem 1. You must gain
permission before using anything else. Assignment work will be tested on a standard Microsoft
Windows XP operating system.

Search Algorithms

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

IMPLEMENTATION PROCEDURE

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

PROGRAMMING INSTRUCTIONS

In this programming, you will have to make decisions about how to solve puzzle problems, states,
nodes, etc. You need to implement the following search algorithms:
Search Type Description Method
Depth-first search Select one option, try it, go back when there are
no more options

DFS

Breadth-first search Expand all options one level at a time BFS
Best-first (F=g+h) Take the best (weighted score), okay to go back BEST
A* SEARCH Priority queue sorted according to the heuristic
function

A* SEARCH

Hill climbing( Using
H function only)
Take the best (weighted score), no going back HC


SAMPLE OUTPUT SHOULD LIKE THIS: (NOT CORRECT ANSWER)

Your program should print out the initial state followed by each move operation selected and its
successor state (i.e. both the operator path and the state path).
At the end, it should:
• Print the cost or the total number of positions that the blank had to move
• The number of nodes expanded -not just the ones to the solution path.

For example, given an initial state RGxRG, your program might print the following lines:
GRXRG
MOVE 5 GRGRX
MOVE 4 GRGXR
MOVE 2 GXGRR
5
20
NUMBER NODE EXPANDED is 20. By this you have completed in solving the puzzle.

SEARCH METHODS:

Your program must support four different search strategies: breadth-first search (BFS), depth first
search (DFS), Best first Search , A* (A-star) & Hill Climbing. Each of these search strategies
should be selectable at runtime by using a command-line keyword. Note that you should be
implementing this using a single function, not three different functions i.e.one for each search
strategy.
NOTE: use a next-state queue containing states that have been generated but not-yet visited as your
primary data structure. In such a data structure, BFS implies a FIFO discipline, DFS implies a LIFO
or “stack” discipline, BEST first implies the search with a heuristic that attempts to predict how
close the end of a path is to a solution, so that paths which are judged to be closer to a solution are
extended first., hill climbing implies the best score of the node, & A* implies a priority queue
sorted according to the heuristic function. Also note that you will need a means of avoiding loops
by checking whether or not a state has already been visited. A* combines the cumulative cost so far
g(n) with a guess about the cost of getting to the solution from the current state h(n), using the
evaluation function f(n)= g(n)+h(n).Define g(n) and h(n) such that g(successor(n)) ≥ g(n) and h(n)
is an admissible heuristic (you can’t use h = 0).

