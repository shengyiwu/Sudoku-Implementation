# Sudoku-Implementation (Python)
## Shengyi Wu

This is a time-killer project that I finished during the quarantine time under the COVID-19 situation.
In this "Sudoku-Implementation" project, I implemented a **sudoku** class that fills all empty 
slots/squares in a sudoku board based on the rules of sudoku games.

The classic Sudoku game involves a grid of 81 squares. The grid is divided into nine blocks, 
each containing nine squares. The rules of the game are simple: each of the nine blocks has to contain
all the numbers 1-9 within its squares. Each number can only appear once in a row, column or box. 

The major two components of the sudoku class are **fill_with_confidence** function which fills those 
empty slots that we are 100% sure based on the rules and **fill_random** function which randomly fills
the rest of empty slots with possible numbers till the whole board is finished. The advantage of this 
method is that **fill_with_confidence** limits the randomness by filling the certain slots first. The
time for the whole process of filling ranges from a few milliseconds to at most a few seconds (see code
examples).

To use the class, the input should be a 9x9 matrix of the original sudoku board with empty slots as 0. 

e.g. 
```np.array([[0,0,0,2,6,0,9,5,0],
[5,0,0,0,0,8,2,0,0],
[0,1,2,0,0,0,0,0,7],
[0,4,0,0,5,6,0,0,0],
[0,5,0,0,0,0,0,6,0],
[0,0,0,4,1,0,0,2,0],
[7,0,0,0,0,0,8,3,0],
[0,0,4,3,0,0,0,0,2],
[0,8,1,0,4,2,0,0,0]])
```
Then, the **fill()** function will output the finished board.






