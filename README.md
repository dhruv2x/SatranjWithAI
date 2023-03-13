# Simple chess AI

A simple chess algorithm with alpha-beta pruning and board evaluation with piece-square tables.
Here I have used 4 Concepts

1. Move-generation
2. Board evaluation
3. Minimax
4. Alpha beta pruning.

Step 1 & 2 : Move generation and board visualization
We’ll use the chess.js library for move generation, and chessboard.js for visualizing the board
Also strength of elemnt is also important.
We will choose element which gives the highest value.

![image](https://user-images.githubusercontent.com/84621641/224666658-76300e14-bff7-436a-a1cc-9b957fd87a3e.png)

Step 3 : Minimax

Whichever search technique we use, The awkward fact remains that for a game such as chess a complete search of the associated graph is out of the question.
A value is associated with each position or state of the game.
The player then makes the move that maximizes the minimum value of the position resulting from the opponent's possible following moves.

Step 4 : Alpha beta pruning

Alpha-beta pruning is an optimization method to the minimax algorithm that allows us to disregard some branches in the search tree. This helps us evaluate the minimax search tree much deeper, while using the same resources.
The alpha-beta pruning is based on the situation where we can stop evaluating a part of the search tree if we find a move that leads to a worse situation than a previously discovered move.

Extra Step : Improved evaluation function

The initial evaluation function is quite naive as we only count the material that is found on the board. To improve this, we add to the evaluation a factor that takes in account the position of the pieces. For example, a knight on the center of the board is better (because it has more options and is thus more active) than a knight on the edge of the board.

![image](https://user-images.githubusercontent.com/84621641/224727296-d3fc121c-f447-4ebd-9d11-6b09747af684.png)

