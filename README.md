# TicTacToe
By Andromeda Weir, Areli Morales-Hernandez, Ben Price

This project aims to create a local network multiplayer Tic-Tac-Toe game using socket programming. The game connects two players on the same local network, allowing them to enjoy the classic game with real-time interaction. The core objectives of the project include developing a functional GUI, implementing game logic, and ensuring smooth communication between players over the network.

### Objectives
- Create a local network multiplayer Tic-Tac-Toe game
- Implement a functional GUI for the game
- Program the underlying logic for the game
- Use socket programming to connect a host and opponent on the same network
- Gain experience with socket programming and its implementation

### Features
The game implements several features to ensure smooth gameplay over a local network:
- **Multiplayer functionality**: Connect two players on the same network
- **GUI**: A user-friendly interface using Tkinter
- **Game state synchronization**: Board state is updated in real-time across both players
- **Socket communication**: Player moves and board state are transmitted over the network

### Class Overview
The codebase is split across several Python files. Key classes include:

#### `Main.py`
- Entry point for the game, initializes and runs the game.

#### `TicTacToe.py`
- Contains the `TicTacToe` class, which handles the game logic.
- **Methods**:
  - `takeTurn(player, posX, posY)`: Processes player moves.
  - `getBoardState()`: Returns the current game state.
  - `updateBoardState(newBoardState)`: Updates the board and checks for game-ending conditions.
  - `checkWin(posX, posY)`: Checks if the move results in a win.
  - `resetGame()`: Resets the game state.

#### `TicTacToeGUI.py`
- Manages the GUI using Tkinter.

#### `Connections.py`
- Defines network connections and implements the `formalConnectionInterface`.
- **Classes**:
  - `TicTacToeServer`: Hosts the game and listens for connections.
  - `TicTacToeClient`: Connects to a server and synchronizes the board state.

#### `GameEndException.py`
- Custom exception thrown when a game ends (win or tie).

### Implementation
This project faced several technical challenges, including ensuring proper communication between components and figuring out how to effectively use Tkinter for the GUI. Significant decisions included:
- Choosing Python as the programming language
- Using Tkinter for the GUI
- Representing the game board as a 2D array
- Utilizing GitHub for version control

### Results Analysis
The project successfully demonstrated the viability of socket programming for creating a local multiplayer game. The key features, such as the GUI and network communication, worked as expected, providing an engaging user experience.


