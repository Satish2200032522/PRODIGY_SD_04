# PRODIGY_SD_04

Create a program that solves Sudokupuzzles automatically. The programshould take an input grid representingan unsolved Sudoku puzzle and use analgorithm to fill in the missing numbers.It should use backtracking or othersuitable techniques to explore possiblesolutions and find the correctarrangement of numbers for the puzzle.Once solved, the program shoulddisplay the completed Sudoku grid.

explanation:
Sudoku Solver Program Explanation
Overview:
This program solves a given unsolved Sudoku puzzle using a backtracking algorithm. It fills in the blank spaces (represented by 0s) with the correct numbers according to Sudoku rules.

Main Components:
Validity Check:

The program contains a function to check if a number can be placed at a specific position on the Sudoku grid without violating Sudoku rules.
It ensures the number is not already present in the same row, column, or 3x3 sub-grid.
Sudoku Solver Function:

The program uses a recursive backtracking approach to solve the Sudoku puzzle.
It iterates through each cell in the grid to find an empty cell.
For each empty cell, it tries placing numbers 1 to 9, checking their validity using the validity check function.
If a valid number is found, it is placed in the cell, and the function recursively attempts to solve the rest of the grid.
If placing a number leads to an unsolvable state, it backtracks by resetting the cell to 0 and trying the next number.
This process continues until the entire grid is correctly filled or it is determined that the puzzle has no solution.
Printing the Grid:

A function is provided to print the Sudoku grid in a readable format.
Main Function:

The program initializes a sample unsolved Sudoku grid.
It calls the solver function to attempt to solve the grid.
If the grid is successfully solved, it prints the solved grid.
If no solution is found, it prints a message indicating that the puzzle is unsolvable.
Execution:
The main function runs the solver on the sample grid and displays the result, either showing the solved Sudoku grid or indicating that no solution exists.
