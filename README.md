# ObstacleAvoidanceGame

This is a simple obstacle-avoidance game based on Pygame. The source code and complete executable file have been made publicly available for playing or for learning and modification. You can download the source code in the repository file list. You can download the Chinese and English version of the executable file in the 'releases'.

In this game, you need to control your ball(black) by moving the mouse to avoid being hit by other blocks. There are four modes in this game, which are 'Normal Mode', 'Infinite Level Mode', 'Survival Mode' and 'Special Mode'. The rules of each mode are listed as follows.

## Normal Mode
In Normal Mode, you start with 3 lives. Every 0.2 seconds, there is a 1% chance to spawn a Life Block (+1 life). Hitting a block reduces your life by 1. When life reaches 0, the game ends. In this mode, the level increases every 4 seconds, and with each level, the block speed and spawn rate increase by 5%, up to a maximum of level 20.\nAfter each game round, the game record is saved in personal_data_Normal Mode.xlsx.
<img src="https://github.com/user-attachments/assets/204c5da5-71a7-47ab-8cf0-79bfc3a6404a" height="400" />

## Infinite Level Mode
In Infinite Level Mode, you start with 3 lives. Every 0.2 seconds, there is a 1% chance to spawn a Life Block (+1 life). Hitting a block reduces your life by 1. When life reaches 0, the game ends. In this mode, the level increases every 4 seconds, and with each level, the block speed and spawn rate increase by 5%, with no maximum level limit.\nAfter each game round, the game record is saved in personal_data_Infinite Level Mode.xlsx.
<img src="https://github.com/user-attachments/assets/3907b000-94f7-4e7a-9768-954f4f4f279b" height="400" />

## Survival Mode
In Survival Mode, you start with 1 life, and no Life Blocks will spawn. Hitting a block ends the game immediately. In this mode, the level increases every 4 seconds, and with each level, the block speed and spawn rate increase by 5%, up to a maximum of level 20.\nAfter each game round, the game record is saved in personal_data_Survival Mode.xlsx.
<img src="https://github.com/user-attachments/assets/a3c08b95-5ab8-4fb6-a25a-34e49a81c916" height="400" />

## Special Mode
In Special Mode, you start with 3 lives. Every 0.2 seconds, there is a 1% chance to spawn a Life Block (+1 life). Hitting a block reduces your life by 1. The game ends when your life reaches 0 or when you hit a Bomb (a red-gray circle). In this mode, the level increases every 4 seconds, and with each level, the block speed and spawn rate increase by 5%, up to a maximum of level 20.\nThis mode also has two special blocks: Ice Block (blue square) slows down all blocks and bombs by half, and Ball Acceleration Block (golden square) increases your ball movement speed by 3x. Both effects last for 3 seconds.\nAfter each game round, the game record is saved in personal_data_Special Mode.xlsx.
<img src="https://github.com/user-attachments/assets/60b22ec0-bc11-4a4d-bc56-d1fef19e3041" height="400" />


# 避障游戏

这是一个基于Pygame的简单避障游戏。源代码及完整的可执行文件已经被发布，可用于游玩或学习与修改。你可以在代码仓库中下载源代码，并可以在‘releases’中下载中文及英文版本的游戏可执行文件。

在本游戏中，你需要控制通过移动鼠标控制你的黑色小球避免其碰到其他的石块。游戏中共有四种模式，分别是‘普通模式’、‘无限等级模式’、‘生存模式’和‘特殊模式’。每种模式的规则如下。

## 普通模式
普通模式中，你初始会有3条命，每0.2秒会有1%的概率刷新出生命石块（生命+1），撞到石块生命-1，生命为0游戏结束。该模式中，每隔4秒等级提升一次，每级石块速度及生成速度提升5%，最高20级。\n在每轮游戏结束后，游戏记录保存在personal_data_{selected_mode}.xlsx文件中。
        if selected_mode == '':
            messagebox.showinfo("普通模式", f"")
        elif selected_mode == '无限等级模式':
            messagebox.showinfo("无限等级模式", f"{selected_mode}中，你初始会有3条命，每0.2秒会有1%的概率刷新出生命石块（生命+1），撞到石块生命-1，生命为0游戏结束。该模式中，每隔4秒等级提升一次，每级石块速度及生成速度提升5%，没有最高等级限制。\n在每轮游戏结束后，游戏记录保存在personal_data_{selected_mode}.xlsx文件中。")
        elif selected_mode == '生存模式':
            messagebox.showinfo("生存模式", f"{selected_mode}中，你初始会有1条命，且不会刷新出生命石块，撞到石块即游戏结束。该模式中，每隔4秒等级提升一次，每级石块速度及生成速度提升5%，最高20级。\n在每轮游戏结束后，游戏记录保存在personal_data_{selected_mode}.xlsx文件中。")
        elif selected_mode == '特殊模式':
            messagebox.showinfo("特殊模式", f"{selected_mode}中，你初始会有3条命，每0.2秒会有1%的概率刷新出生命石块（生命+1），撞到石块生命-1，生命为0或撞到炸弹（红灰相间的圆）游戏结束。该模式中，每隔4秒等级提升一次，每级石块速度及生成速度提升5%，最高20级。\n该模式中还有两种特殊石块，冰冻石块（蓝色方形）可使所有石块及炸弹速度减半，加速石块（金色方形）可使你控制的小球移速快3倍，两者效果均持续3秒。\n在每轮游戏结束后，游戏记录保存在personal_data_{selected_mode}.xlsx文件中。")
