# vikas_AI_431MZ

---------------------BACKGROUND--------------------------------

Fence and conquer is a two player game, where both the players are bots. A color is assigned to each bot.
There is a grid of square cells of size 
N
×
N
. At the start of the game all the cells are empty.
When the game starts, the bots are assigned random distinct locations within the grid. These locations get the color of the bot.


--------------------OBJECTIVE-------------------------------------

The objective of a bot is to conquer more cells than its competitor bot.

-------------------MOVING WITHING THE GRID------------------------

One of the bots gets to make the first move.
The bots take turns to move a step to the left, right, up, or down within the grid. A bot may also choose not to move.
At a grid edge, if a bot makes another move towards the edge, it will wrap around and emerge from the opposite edge.

--------------------Conquering cells:-----------------------------

If a bot moves into an empty cell, the empty cell gets conquered and gets the color of the bot.
If a bot makes a rectangle such that all the cells within the rectangle are empty, all those empty cells also get 'conquered' and get the color of the bot. Constraint: A bot can only conquer rectangles of size up to 
6
×
6
 cells in this manner.
A bot can move to any cell in the grid, but cannot conquer an already conquered one. That is, if a cell gets colored, it's color cannot be changed even if a bot of different color moves through it.

-------------------Timing constraints:----------------------------

There is a 10 second stop clock for each bot. That is, a bot gets 10 seconds of aggregate time to make its moves within a game.
The clock for a bot stops whenever it waits for the other bot to make a move.
The bot that runs out of time first, loses the game.
In case both bots end up conquering the same number of cells in a game, the bot that consumes the least time to make all its moves is the winner.
