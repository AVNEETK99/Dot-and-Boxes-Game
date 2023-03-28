# Dot-and-Boxes-Game

Dot and Boxes is a classic pencil-and-paper game for two players. The game is played on a rectangular grid of dots, and each player takes turns connecting a pair of adjacent dots with a line. When a player completes a box (by connecting the fourth side of a square), they write their initial in the box and get to take another turn. The game continues until no more lines can be drawn, and the player with the most boxes at the end of the game wins. Dot and Boxes is a simple yet challenging game that is often played as a fun pastime or as a way to develop strategic thinking skills.

## Instructions to run the game

* Open the Github repository where the game code is hosted.

* Click on the green "Code" button and then select "Download ZIP" to download the code as a ZIP file.

* Extract the ZIP file to a folder on your computer.

* Open a command prompt or terminal window and navigate to the folder where you extracted the code.

* Type ```python index.py``` and press Enter to start the game.

* Follow the prompts to play the game.

## Functionality of the code

* The code begins with importing the ```tkinter``` and ```numpy``` libraries. It defines various constants for the size of the board, the number of dots, symbol size, symbol thickness, dot color, player colors, and other display-related parameters.

* A class named ```Dots_and_Boxes``` is defined, which has various methods to play the game, such as refreshing the board, marking the box, updating the board, checking whether the grid is occupied or not, converting the grid to logical position, etc.

* The constructor method of the class creates the window and canvas for the game, binds the left button of the mouse to a click event, and sets the player 1 to start the game. It also calls the ```refresh_board()``` method and ```play_again()``` method.

* The ```play_again()``` method is used to reset the board, set the player who starts the game, and display the turn text. It also initializes the board_status, row_status, and col_status arrays.

* The ```is_grid_occupied()``` method checks whether a grid position is occupied or not. It takes the logical position of the grid and its type (row or column) as input parameters and returns a boolean value.

* The ```convert_grid_to_logical_position()``` method takes the grid position as an input parameter and returns its logical position on the board.

* The ```mark_box()``` method is used to shade the box with a color if it is marked.

* The ```update_board()``` method is used to update the board with the player's move. It takes the logical position and type of the move as input parameters and updates the board status, row status, and column status accordingly.

* The ```is_gameover()``` method checks whether the game is over or not by checking the row and column status of the board.

* The ```make_edge()``` method is used to create an edge on the board. It takes the logical position and type of the edge as input parameters and draws a line on the canvas. It also sets the color of the line according to the current player's turn.
