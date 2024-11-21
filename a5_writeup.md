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

The performance and efficiency of the DFS and BFS compare when solving Sudoku puzzles because the DFS algorithm is more efficient because it performs fewer iterations. The DFS performed 87 for 81, whereas the BFS performed something around 543 for 81. In scenarios where the data being stored is deeper and more complex, the DFS would be preferable because it would find the desired information faster than the BFS. For example, storing information about a person would be a deep stack of info, requiring efficiency to gather whether it's birthday or place of birth, etc. 

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

The choice of data structures impacted the implementation and the functionality of the algorithms because for this assignment, it did not really matter that much how efficient the structure was because we are only looking at a 9*9 board, but in other real world cases there are much larger data bases with more data, efficieny matters. Another structure that you could use is a set. A set is a data structure that represents elements that are not ordered. A set is similar to a dictionary without the order. You also cannot index or slice a set. 


3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

The Sudoku solver could be adapted or extended for a larger puzzle by using a set to increase the efficiency of the program. Along with this, you could maybe make more functions to help narrow down the possible outcomes of the Sudoku board. Lessons can be learned from this assignment about stacks and queues and how to represent data in bot breadth and depth. This is useful for organizing data that is both deep and wide in scope. 