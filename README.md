# ARM - C  
## Reversi game
###The main objective is to implement a version of the well-known classic game Reversi for the STM32F769i Discovery board in C. 
The game state should be shown on the LCD. The touch screen must be used by each player to indicate his move. The SD-Card will be used to store the game’s results. Each player has a timeout to play. Additionally, the internal temperature should be shown on the LCD and updated periodically. The update rates of clocks and acquisitions must be controlled by Timers and the use of Interrupts is mandatory.  

- Read the ARM internal temperature and show it in the LCD. The temperature information should be kept visible at all time in one of the LCD corners and updated every 2 seconds. 
- Create the game board. It has an 8x8 grid that should be drawn in accordance to the available LCD space. Leave some lateral area to show extra data like game status and optional information. 
- Implement cells selection recognition, inside game board, using the Touch Screen. This should match the touched area to the corresponding board cell. 
- Implement the Reversi game, using the interface created in the previous goals. Impossible movements should not be allowed. 
- The game start should be selected through a menu/button on LCD. The push-button available on board is used to cancel a running game, returning to an initial pre-game state. 
- At the end of each game, save in SD-Card some statistics like: winner, punctuations, total game duration, and other information that you consider relevant. 
- Introduce a feature that limits the amount of time (20 seconds) that each player has to make his move. When the time runs out, the game automatically transfers the player order to the opponent. After triggering three timeouts, a player loses the game. A countdown timer should be shown in the LCD. 
- Add a clock to show the total game duration. 
- Add an automatic ARM player. This game mode should be chosen in an initial game menu.