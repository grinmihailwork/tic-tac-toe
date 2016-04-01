#Tic-Tac-Toe in Python

Algorithm
============================
I thought of porting my C program for tic-tac-toe written several years ago to Python since C is considered too main stream nowadays. The game is played by recursing down the game/decision tree and choosing the best move that maximizes the gain and minimizes the loss. Running time is proportional to number of plies or the lookahead. Minimax algorithm belongs to branch and bounds class of algorithm.

TODO
============================
* Python lists are immutable and deep copy is being done when every new move is generated. Need to eliminate the list and use the tuple (x,y) for array indexing
* Running time is proportional to number of plies. Dynamic look-ahead based on the situation of the game might improve the running time
* Alpha-beta pruning can further eliminate the non sub optimal branches while recursing down the game tree
* Computer always gets to play second
* Too bored to do some bounds checking of input at this point in time
* Though the computer employs the perfect player strategy, it might play some dumb moves when it knows all possible moves are a loss
* The scoring strategy should be a function of the current depth of the game tree to solve the above problem (Too lazy to fix)
* Randomize the moves when there are more than one possible best move

How to play ?
===========================
* Tic-tac-toe is a python script. Invoke the game using the command 'python tic-tac-toe.py'
* Gameboard is nothing but a 3X3 matrix initially with elements as '-'
* Players choice is 'X' and computers choice is 'O'
* Player has to input X Y i.e basically they are nothing but the index of 3X3 matrix.
* The allowed range for input is X >=1 && X <= 3 and similarly Y>=1 && Y <=3
* Game can be either won, lost or drawn

Example output
===========================
```
Welcome to Tic-Tac-Toe
Players choice is X and my choice is O
- - -

- - -

- - -

Enter (row, column)

1 1
X - -

- - -

- - O

Enter (row, column)

1 2
X X O

- - -

- - O

Enter (row, column)

2 3
X X O

- - X

O - O

Enter (row, column)

3 2
You lose
X X O

- O X

O X O

Press y to continue; any other key to exit
```

