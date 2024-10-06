# Slot Machine Game
This is a simple command-line slot machine game built with JavaScript. Players can deposit money, place bets, and spin the slot machine to see if they win. The game allows players to bet on up to three lines, and winnings are calculated based on matching symbols across those lines.

## Features
1. Deposit Money: Players deposit an initial amount to play the game.
2. Bet on Lines: Players choose how many lines (1 to 3) they want to bet on.
3. Place a Bet: Players specify the bet amount for each line.
4. Spin the Slot Machine: The game generates random symbols on a 3x3 grid.
5. Win or Lose: The game checks if symbols match across the chosen lines.
5. Winnings: Players receive winnings based on the symbol values and the bet.
6. Play Again: Players can decide whether to play another round or quit.
## How to Play
1. Deposit Money
When you start the game, you will be prompted to enter a deposit amount. This is the money you will use to place your bets.

2. Bet on Lines
Choose how many lines you want to bet on (between 1 and 3). Each line increases the chance of winning, but it also increases the cost of your bet.

3. Place Your Bet
Enter the amount you want to bet per line. The total bet will be the amount per line multiplied by the number of lines you selected.

4. Spin the Slot Machine
The slot machine will randomly generate a grid of symbols (A, B, C, D) across 3 rows and 3 columns. Each symbol has different odds and values:

- A: 2 symbols, value = 5
- B: 4 symbols, value = 4
- C: 6 symbols, value = 3
- D: 8 symbols, value = 2
5. Winning or Losing
If all symbols on a bet line match, you win based on the symbol's value and your bet. The more valuable the symbol, the more you win.

6. Collect Winnings or Play Again
After each spin, the game will display your winnings and update your balance. If your balance reaches zero, the game ends. You can choose to play again as long as you have a positive balance.

## Running the Program
1. Install prompt-sync if you don't have it:

```
npm install prompt-sync
```
2. Run the program:


```
node slot_machine.js
```

## Code Structure
- deposit(): Prompts the player to enter a deposit amount.
- getNumberOfLines(): Asks the player to select how many lines to bet on (1 to 3).
- getBet(): Prompts the player to enter a bet amount per line.
- spin(): Generates random symbols for the slot machine.
- transpose(): Reorganizes the columns into rows for easier comparison.
- printRows(): Displays the grid of symbols to the player.
- getWinnings(): Calculates the player's winnings based on matching symbols.
- game(): Manages the game loop, including balance updates, spins, and playing again.

### Example Gameplay
1. Enter a deposit amount:
Enter a deposit amount: 50

2. Select the number of lines to bet on:
Enter the number of lines to bet on (1-3): 3

3. Enter the bet per line:
Enter the bet per line: 5

4. The slot machine spins:

```
C | A | D
B | A | B
D | A | C
```
5. You win or lose:
You won, $15

6. Play again or exit:
Do you want to play again (y/n)?

## License
This project is licensed under the MIT License.

Enjoy the game and good luck! 🎰
