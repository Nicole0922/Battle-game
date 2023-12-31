# battle game
In this game, players move around a game board and collect items for fighting. They may also "step" on a bomb and get hurt. When the two players meet, they will battle using the collected items, and the game will end.

Game Logic:
The following shows the general logical flow of the game. We will also refer the game board as a grid and each position as a (grid) cell.

1. A game board consists of BOARD_SIZE * BOARD_SIZ grid cells (initialized as 7x7 in this project).
2. Game pieces include players and items, which can be an attack item, a defense item or a bomb.
3. Two players take turns to move around the board.
4. If a player moves to a grid cell occupied by an item (other than a bomb), the player picks it up for later use.
5. If a player moves to a grid cell occupied by a bomb, the player will get hurt (and his hp will be reduced) or even die. If one player dies, the game will end and 6. the other player becomes the winner.
7. When the two players meet, they will battle using their collected items until one player dies (with hp <= 0), or no one has attack items anymore.
8. After the battle, the game will end and the player with higher hp is the winner. If the two players have the same hp, the game ends in a draw.
