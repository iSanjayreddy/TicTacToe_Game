# TicTacToe_Game
This is the famous TicTacToe game that i have built using python and with GUI(Graphical User Interface) using module Tkinter
# Tic-Tac-Toe Game

This is a simple implementation of the Tic-Tac-Toe game using the Tkinter library in Python. The game allows two players to take turns and compete against each other. The code is organized into two classes: `TicTacToeGame` and `TicTacToeBoard`.

## TicTacToeGame Class
The `TicTacToeGame` class represents the game logic and state. It keeps track of the players, the current player, the game board, and determines the winner.

### Methods:
- `__init__(self, players=DEFAULT_PLAYERS, board_size=BOARD_SIZE)`: Initializes the game with the given players and board size. It sets up the initial state of the game board.
- `_setup_board(self)`: Sets up the game board by creating a 2D list of moves.
- `_get_winning_combos(self)`: Generates a list of winning combinations on the board.
- `toggle_player(self)`: Toggles the current player to the next player.
- `is_valid_move(self, move)`: Checks if the given move is valid or not.
- `process_move(self, move)`: Processes the current move and checks if it results in a win.
- `has_winner(self)`: Returns `True` if the game has a winner, and `False` otherwise.
- `is_tied(self)`: Returns `True` if the game is tied, and `False` otherwise.
- `reset_game(self)`: Resets the game state to play again.

## TicTacToeBoard Class
The `TicTacToeBoard` class represents the graphical user interface (GUI) of the game using the Tkinter library.

### Methods:
- `__init__(self, game)`: Initializes the game board window and creates the necessary GUI elements.
- `_create_menu(self)`: Creates the menu bar with options to play again or exit the game.
- `_create_board_display(self)`: Creates the display area to show the game status.
- `_create_board_grid(self)`: Creates the game board grid with buttons for each cell.
- `play(self, event)`: Handles a player's move when a button is clicked.
- `_update_button(self, clicked_btn)`: Updates the appearance of a button after a valid move.
- `_update_display(self, msg, color="black")`: Updates the display with the given message and color.
- `_highlight_cells(self)`: Highlights the cells that resulted in a win.
- `reset_board(self)`: Resets the game board to play again.

## Running the Game
The `main` function creates an instance of the `TicTacToeGame` class and a `TicTacToeBoard` instance with the game object. It then starts the game's main loop.

To play the game, run the script, and a window will open with the Tic-Tac-Toe game board. Two players can take turns by clicking on the empty cells. The game will display the current player's turn and announce the winner or a tie when appropriate. You can also reset the game board or exit the game using the menu options.

Have fun playing Tic-Tac-Toe!
