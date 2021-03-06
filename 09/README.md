## Exercise 9

### Problem

In this problem we want to build a [Tic Tac Toe game](https://en.wikipedia.org/wiki/Tic-tac-toe).
The goal is *not* to build an artificial intelligence to play against, but to let two players play together.

The program must do, for each player's turn:
* display the board
* ask the player his move (the cell number)
* detect if the move is illegal, and keep asking the user for a legal move
* detect if the game is finished, either because the player has won or the board is full

The board could be numbered like this, to identify each cell:
```
1 | 2 | 3
4 | 5 | 6
7 | 8 | 9
```
Then, the game could be played like this
```
X | X | O
. | O | .
. | . | .

> Player O, what is your move? 7
Player O won against player X!
```
### Help

* User input should *not* be able to break the program (some exception-catching must be done :wink:).
* The board could be represented with a class `Board`, with at least the following methods:
    * `board.update(player, move)`
    * `board.is_full()`
    * `board.has_won(player)`
    * `board.show()`
* The board could store cells data in a list of 9 elements (this may be simpler than a 2D list)

### Bonus

Cells numbers could be reversed from top to bottom to match the numpad layout.
```
7 | 8 | 9
4 | 5 | 6
1 | 2 | 3
```
