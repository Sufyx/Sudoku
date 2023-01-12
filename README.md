## Sudoku

[Project deployment link](https://ag-sudoku.onrender.com/) <br>

![demo](demo.gif)


A game of Sudoku.
Featuring various difficulties, hints, mistake checks, optional user creation, and more.
The boards are randomly generated on the fly, using recursive functions.

- - - - -
#### Features:

- **Front Page** Guest and Sign-In options. <br> 
Enter as guest or sign-up/log-in with a user.\
A registered user will be able to choose a difficulty, while a guest can only play in easy mode.

- **Difficulty settings**: The user may choose between 3 difficulty settings, which affects the number of hidden tiles on the board as well as the number of hints available to the user. ie:\
 - Easy: 20 tiles hidden, 5 hints available.\
 - Normal: 40 tiles hidden, 4 hints available.\
 - Hard: 60 tiles hidden, 3 hints available.\
 - Empty: A completely empty board, no hints. Used in case a user wants, for example, to solve a Sudoku game from a newspaper or other source they may be stuck on. So they can replicate it using the Empty setting and get a solution using this app's features. 

- **'Check' button**:
Causes every row, column or square containing a mistake (a number appearing more than once) to be marked in red.

- **'Hint' button**:
Will reveal one hidden tile with a correct number.\
*Note*: 'A correct number' doesn't only mean a number that will cause no immediate errors, but one that can positively lead to a fully solved board. The only way to guarantee this is to solve the entire existing board (behind the scenes) and to extract the value for the hint from the full solution.

- **'Again' button**: Clear all user input and restart the same board.

- **'New Board' button**: Start a new cleared board with different values on the same difficulty level.

- **'Finish' button**: Check if user has successfully solved the current board, and display a corresponding message.

- **'Show Solution' button**: Fully solves the current board. If possible, will complete what the user started. As in, will try to solve the board while keeping as much of the user input as possible. Any user input that leads to a dead end will first be cleared, only then a full solution will be calculated.\
*Note*: This feature does not use a copy of the initial board that was created prior to hiding the necessary number of tiles as the correct solution. Doing so is a mistake since a board with a certain number of hidden tiles can have multiple solutions. Instead it calculate a solution every time.

- **'Change Level'**: Returns the user to the difficulty selection screen. Current game's progress will not be saved.

- **'Back to main'**: Returns to the entrance login screen. Current user will be logged out.


-----
Did you know? 
<br>
There are 6,670,903,752,021,072,936,960 different combinations for a sudoku board