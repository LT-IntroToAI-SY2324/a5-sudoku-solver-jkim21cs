# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

    The BFS algorithm is more efficient than the DFS since it explores  all the nodes on the same "level" before moving on, this allows the algorithm to find a solution the fastest while DFS searches through a lot more possibilities before backtracking causing the algorithm yo take more time. I didnt really have an answer other than efficieny so I searched it up. DFS does not require as much memory as BFS which may be helpful when memory is a critical resource in a system. 


2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

    The choice of data structures impact the implementation and functionality of the algorithms because the algorithms have different ways of "tracking" information. For example, BFS typically uses a queue to maintain the order of nodes being explored. 

    Searched up:
        Deep search: Adjacency List, graph representation, and path stack 
        Quickest search: Visited set/ Array, Parent pointers, hash set

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be ap, andplied to real-world problem-solving or optimization challenges?

    The Sudoku solver could be used to solve the sliding puzzles as each sqaure of the puzzle must be arranged by a certain sequence to restore the pieces to their original places. 

    Certain data structures help to optimize different algorithms that focus on different purposes. So understanding the strengths of algorithms help to optimize solution solving whether it be for finding the quickest solutions (ie. epidemiology) or find the best solution (ie.data mining)

