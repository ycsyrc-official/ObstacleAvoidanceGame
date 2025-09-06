# ObstacleAvoidanceGame

This is a simple obstacle-avoidance game based on Pygame. The source code and complete executable file have been made publicly available for playing or for learning and modification. You can download the source code in the repository file list. You can download the Chinese and English version of the executable file in the 'releases'.

In this game, you need to control your block(black) to avoid being hit by other blocks. There are four modes in this game, which are 'Normal Mode', 'Infinite Level Mode', 'Survival Mode' and 'Special Mode'. The rules of each mode are listed as follows.

## Normal Mode
In Normal Mode, you start with 3 lives. Every 0.2 seconds, there is a 1% chance to spawn a Life Block (+1 life). Hitting a block reduces your life by 1. When life reaches 0, the game ends. In this mode, the level increases every 4 seconds, and with each level, the block speed and spawn rate increase by 5%, up to a maximum of level 20.\nAfter each game round, the game record is saved in personal_data_Normal Mode.xlsx.

## Infinite Level Mode
In Infinite Level Mode, you start with 3 lives. Every 0.2 seconds, there is a 1% chance to spawn a Life Block (+1 life). Hitting a block reduces your life by 1. When life reaches 0, the game ends. In this mode, the level increases every 4 seconds, and with each level, the block speed and spawn rate increase by 5%, with no maximum level limit.\nAfter each game round, the game record is saved in personal_data_Infinite Level Mode.xlsx.

## Survival Mode
In Survival Mode, you start with 1 life, and no Life Blocks will spawn. Hitting a block ends the game immediately. In this mode, the level increases every 4 seconds, and with each level, the block speed and spawn rate increase by 5%, up to a maximum of level 20.\nAfter each game round, the game record is saved in personal_data_Survival Mode.xlsx.

## Special Mode
In Special Mode, you start with 3 lives. Every 0.2 seconds, there is a 1% chance to spawn a Life Block (+1 life). Hitting a block reduces your life by 1. The game ends when your life reaches 0 or when you hit a Bomb (a red-gray circle). In this mode, the level increases every 4 seconds, and with each level, the block speed and spawn rate increase by 5%, up to a maximum of level 20.\nThis mode also has two special blocks: Ice Block (blue square) slows down all blocks and bombs by half, and Ball Acceleration Block (golden square) increases your ball movement speed by 3x. Both effects last for 3 seconds.\nAfter each game round, the game record is saved in personal_data_Special Mode.xlsx.

