#Tic-Tac-Toe

Algorithm
============================
The game is played by recursing down the game/decision tree and choosing the best move that maximizes the gain and minimizes the loss. Running time is proportional to number of plies or the lookahead. 

TODO
============================
* Python lists are immutable and deep copy is being done when every new move is generated. Need to eliminate the list and use the tuple (x,y) for array indexing.
* Running time is proportional to number of plies. Dynamic look-ahead based on the situation of the game might improve the running time.
* Alpha-beta pruning can further eliminate the non sub optimal branches while recursing down the game tree.


