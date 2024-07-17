# Slot Machine

This is a JavaScript-based slot machine game with 4 rows and 4 columns. Users can input money to play and continue playing as long as their deposit is more than 0.

## Features

- 4x4 slot machine grid
- User input for deposit amount
- Continue playing as long as deposit > 0

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/slotmachine.git
    ```
2. Navigate to the project directory:
    ```sh
    cd slotmachine
    ```
3. Install dependencies:
    ```sh
    npm install
    ```

## Usage

1. Start the game:
    ```sh
    node Slotmachine.js
    ```

2. Follow the on-screen instructions to input your deposit and play the game.

## Code Explanation

### Constants and Symbol Definitions

- `ROWS` and `COLS`: Defines the dimensions of the slot machine grid (4x4).
- `SYMBOLS_COUNT`: An object defining the count of each symbol in the slot machine.
- `SYMBOLS_VALUES`: An object defining the payout value of each symbol.

### Functions

#### `deposit()`
Prompts the user to enter a deposit amount and validates the input. It keeps asking until a valid positive number is entered.

#### `getNumberOfLines()`
Prompts the user to enter the number of lines to bet on (up to 4). It keeps asking until a valid number is entered.

#### `getBet(balance, lines)`
Prompts the user to enter the bet amount per line. It validates the input to ensure it is a positive number and does not exceed the available balance divided by the number of lines.

#### `spin()`
Generates the slot machine's reel symbols by randomly selecting symbols based on their defined counts. It returns a 2D array representing the reels.

#### `transpose(reels)`
Transposes the reels array to get a row-wise representation of the slot machine grid.

#### `printRows(rows)`
Prints the rows of the slot machine grid.

#### `getWinnings(rows, bet, lines)`
Calculates the total winnings based on the bet amount, number of lines, and the symbols in each row. It returns the total winnings and the winning lines.

#### `game()`
Main game loop that handles the user deposit, betting, spinning the reels, calculating winnings, and updating the balance. The game continues as long as the user has a positive balance.

## Project Structure

- `.git`: Contains the git repository metadata.
- `node_modules`: Contains the project dependencies.
- `package-lock.json`: Contains the locked dependency tree.
- `package.json`: Contains project metadata and dependencies.
- `Slotmachine.js`: Main JavaScript file for the slot machine game.



## Contact

If you have any questions or suggestions, feel free to contact me at mohammedmutasim13@gmail.com.
