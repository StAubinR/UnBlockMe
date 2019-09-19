# UnBlockMe
UnBlockMe Webpage to help, solve, validate, edit, play, create, save and load UnBlockMe Game.

This is just one html page under 1000 lines with javascript to test algorithms to solve UnBlockMe puzzles.  I tried to keep things as simple as possible without any fancy javascript stuff.  I focus on algorthms that persons can use to solve puzzles.  If anybody has more fun coding a Puzzle than to solve one, let me know.

This program has the following options:
1) Edit/Play: Drag and drop blocks to build your own puzzle or play.
2) Show/Hide Tips: Show how to solve a UnBlockMe.
3) Analyse: Count how many solutions you have and give the longest path for this puzzle.
4) Clear: Empty UnBlockMe grid before you enter your own puzzle.
5) New Game: Create/generate a new easy to solve UnBlockMe puzzle.
6) Save: Save your game using local storage.
7) Load: Load a game using local storage.

This javascript program uses a very simple algorithm to solve UnBlockMe puzzles.  It uses a big array to store every possible move and uses it to find the shortest path.  I tried 4 or 5 different algorithms to solve a UnBlockMe puzzles, but this one is very simple to understand and fast enough.  All blocks are stored in an array with their positions and their shapes.  I encoded these blocks in an array and used it as a key for my big array to store a distance path.

The basic algorithm is:
1) Start with one position of blocks, store 1 in the big array, and $level = 1.
2) For every possible move from $level store $level+1 in the big array.
3) When it is done, find every winning position and store 1, otherwise store 0.
4) Repeat the same process as #2.

The game starts with the longest path I found.  It is a 60 moves game you can play using tips box.

TO DO: Improve my process to create new games.