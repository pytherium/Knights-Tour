# Knights-Tour
Given an (N x N) board with the Knight placed on the first block of an empty board. Moving according to the rules of chess, the knight must visit each square on the board exactly once. Each square on the board will be marked with the move number on which it is visited.

# The Naive solution
The Naive solution to the problem consists of trying every possible configurations and output a one that follows the problem constraints. This is not a good solution to the problem, as the board has 81 squares, each with 9 possible entries. This amounts to just under 9^81 possible board setups that the algorithm would have to go through in order to find the correct solution, which is not an effiicient way to solve the problem.

# Using a Backtracking Algorithm
The problem is first solved using the backtracking algorithm. This works in an incremental way to determine the solution - the algorithm starts with an empty vector solution and adds items one by one. If adding the current item violates the problem constraint, then the item is removed and an alternative item is tried. If adding an item doesn’t violate constraints then each is added recursively one by one. Otherwise, the algorithm backtracks to the previous step and removes that item to try more combinations.

# Using Warnsdorff’s Algorithm
Another way to solve this problem is to use heuristics (a method which chooses the next move with the fewest possible options, in order to waste less time checking through possible outcomes). 
