# Tic Tac Toe Game

A simple Tic Tac Toe game built with HTML, CSS, and JavaScript. Play against a basic computer opponent as you try to line up three of your symbols in a row.

---

## Features

- **Symbol Selection:**  
  Choose your symbol (X or O) before the game starts.

- **Interactive Game Board:**  
  A 3x3 grid where players can click cells to place their symbol.

- **Basic Computer AI:**  
  The computer randomly selects an empty cell to make its move.

- **Win & Draw Detection:**  
  Automatically checks for winning combinations or a draw after every move.

- **Status Updates:**  
  Displays messages indicating whose turn it is and the game result.

- **Automatic Reset:**  
  The game resets after a win or a draw, allowing for a new game.

---

## Project Structure

TicTacToe/ ├── index.html # Contains all HTML, CSS, and JavaScript for the game


---

## How to Play

1. **Open the Game:**  
   Open `index.html` in your web browser.

2. **Select a Symbol:**  
   Click on "Play as X" or "Play as O" to choose your symbol.  
   - If you choose **X**, you'll play first.  
   - If you choose **O**, the computer starts.

3. **Make Your Move:**  
   Click an empty cell on the game board to place your symbol.

4. **Computer's Turn:**  
   After your move, the computer will choose a random empty cell for its move.

5. **Game Outcome:**  
   The game automatically checks for wins or a draw:
   - **Win:** A winning combination (row, column, or diagonal) ends the game.
   - **Draw:** If all cells are filled without a winner, the game is a draw.
   
6. **Reset:**  
   After a win or a draw, the game displays the result and resets after a short delay.

---

## Code Breakdown

### 1. Symbol Selection

- **Function:** `selectSymbol(symbol)`  
  - **Purpose:** Sets the player's symbol and assigns the opposite symbol to the computer.
  - **Behavior:** Hides the symbol selection buttons, shows the game board, and determines whose turn is first (player goes first if symbol is X).

### 2. Handling Cell Clicks

- **Function:** `handleCellClick(index)`  
  - **Purpose:** Processes the player's move.
  - **Behavior:**
    - Verifies that the game is active, the clicked cell is empty, and it's the player's turn.
    - Updates the board with the player's symbol.
    - Checks if the move results in a win or a draw.
    - If not, toggles the turn to the computer and updates the status message.

### 3. Computer Move

- **Function:** `computerMove()`  
  - **Purpose:** Lets the computer make a move.
  - **Behavior:**
    - Collects indices of all empty cells.
    - Randomly selects an empty cell and places the computer's symbol there.
    - Checks for a win or draw; if neither, it switches the turn back to the player.

### 4. Outcome Detection

- **Function:** `checkWin(symbol)`  
  - **Purpose:** Determines if the provided symbol has achieved a winning combination.
  - **Mechanism:** Evaluates predefined winning patterns (rows, columns, diagonals).

- **Function:** `checkDraw()`  
  - **Purpose:** Checks if all cells are filled, indicating a draw.

- **Function:** `endGame(message)`  
  - **Purpose:** Ends the game by displaying a win/draw message and then resetting the game after a delay.

### 5. UI Updates

- **Function:** `updateCellUI(index)`  
  - **Purpose:** Updates the visual content of a cell based on the game state.

- **Function:** `updateStatus()`  
  - **Purpose:** Updates the status message to show whether it's the player's turn or the computer's turn.

### 6. Resetting the Game

- **Function:** `resetGame()`  
  - **Purpose:** Resets the game state and UI elements to allow a new game.
  - **Behavior:** Clears the board, resets internal variables, and shows the symbol selection screen.

---

## Future Enhancements

- **Smarter AI:**  
  Implement a more strategic approach for the computer moves.

- **Score Tracking:**  
  Keep track of wins, losses, and draws over multiple rounds.

- **Responsive Design:**  
  Enhance the UI to perform well on mobile devices.

- **Restart Option:**  
  Provide a manual restart button without waiting for the automatic reset delay.

---

## License

This project is open-source and available under the **MIT License**.
# Tic-Tac-Toe
