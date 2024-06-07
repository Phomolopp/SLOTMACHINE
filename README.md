This is a simple slot machine game implemented in Python. The game allows the player to deposit money, place bets on up to three lines, and spin the slot machine to win or lose money based on the outcome. The code demonstrates basic principles of user input, randomization, and simple game mechanics.

Features
Deposit System: Allows the player to deposit money to their balance before playing.
Betting Mechanism: The player can bet on up to three lines, with customizable bet amounts within a specified range.
Slot Machine Simulation: Randomly generates slot machine results using a predefined set of symbols and their frequencies.
Win Checking: Determines if the player has won based on matching symbols in the specified lines and calculates the winnings accordingly.
Balance Update: Adjusts the player's balance based on the total bet and the winnings from the spin.
Game Rules
The slot machine has 3 rows and 3 columns.
The symbols available are "A", "B", "C", and "D", each with different frequencies and values:
"A": Appears 2 times, value 5
"B": Appears 4 times, value 4
"C": Appears 6 times, value 3
"D": Appears 8 times, value 2
The player wins if all symbols in a line match. The winnings are calculated by multiplying the symbol's value by the bet amount.
Code Description
Constants and Variables
MAX_LINES: Maximum number of lines the player can bet on (3).
MAX_BET: Maximum bet amount per line ($100).
MIN_BET: Minimum bet amount per line ($1).
ROWS and COLS: Dimensions of the slot machine (3x3).
symbol_count: Dictionary representing the frequency of each symbol.
symbol_value: Dictionary representing the value of each symbol.
Functions
check_winnings(columns, lines, bet, values):

Checks for winning lines in the slot machine columns.
Calculates the total winnings based on matching symbols and bet amount.
Returns the total winnings and a list of winning lines.
get_slot_machine(ROWS, COLS, symbols):

Generates a random slot machine layout based on the provided symbols and their frequencies.
Returns the slot machine columns.
print_slot_machine(columns):

Prints the slot machine columns in a formatted manner.
deposit():

Prompts the player to deposit money.
Returns the deposited amount.
get_Number_of_lines():

Prompts the player to enter the number of lines to bet on.
Returns the number of lines.
get_bet():

Prompts the player to enter the bet amount per line.
Returns the bet amount.
spin(balance):

Handles the betting and spinning process.
Updates the player's balance based on the bet and winnings.
Returns the net balance change.
main():

Main game loop.
Handles user input for playing or quitting the game.
Manages the player's balance throughout the game.
How to Play
Run the script.
Deposit money to start the game.
Enter the number of lines to bet on (1-3).
Enter the bet amount per line.
Spin the slot machine and see the results.
The game continues until the player decides to quit by entering 'q'.
The final balance is displayed when the player quits the game.
