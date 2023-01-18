## Description

<div><p>Galois is one of the strongest chess players of Byteforces. He has even invented a new variant of chess, which he named «PawnChess».</p><p>This new game is played on a board consisting of 8 rows and 8 columns. At the beginning of every game some black and white pawns are placed on the board. The number of black pawns placed is not necessarily equal to the number of white pawns placed. </p><center> <img class="tex-graphics" src="file://1IrVJIVj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Lets enumerate rows and columns with integers from 1 to 8. Rows are numbered from top to bottom, while columns are numbered from left to right. Now we denote as <span class="tex-span">(<i>r</i>, <i>c</i>)</span> the cell located at the row <span class="tex-span"><i>r</i></span> and at the column <span class="tex-span"><i>c</i></span>.</p><p>There are always two players A and B playing the game. Player A plays with white pawns, while player B plays with black ones. The goal of player A is to put any of his pawns to the row <span class="tex-span">1</span>, while player B tries to put any of his pawns to the row <span class="tex-span">8</span>. As soon as any of the players completes his goal the game finishes immediately and the succeeded player is declared a winner.</p><p>Player A moves first and then they alternate turns. On his move player A must choose exactly one white pawn and move it one step upward and player B (at his turn) must choose exactly one black pawn and move it one step down. Any move is possible only if the targeted cell is empty. It's guaranteed that for any scenario of the game there will always be at least one move available for any of the players.</p><p>Moving upward means that the pawn located in <span class="tex-span">(<i>r</i>, <i>c</i>)</span> will go to the cell <span class="tex-span">(<i>r</i> - 1, <i>c</i>)</span>, while moving down means the pawn located in <span class="tex-span">(<i>r</i>, <i>c</i>)</span> will go to the cell <span class="tex-span">(<i>r</i> + 1, <i>c</i>)</span>. Again, the corresponding cell must be empty, i.e. not occupied by any other pawn of any color.</p><p>Given the initial disposition of the board, determine who wins the game if both players play optimally. Note that there will always be a winner due to the restriction that for any game scenario both players will have some moves available.</p></div><div class="input-specification"><p>The input consists of the board description given in eight lines, each line contains eight characters. Character '<span class="tex-font-style-tt">B</span>' is used to denote a black pawn, and character '<span class="tex-font-style-tt">W</span>' represents a white pawn. Empty cell is marked with '<span class="tex-font-style-tt">.</span>'. </p><p>It's guaranteed that there will not be white pawns on the first row neither black pawns on the last row.</p></div><div class="output-specification"><p>Print '<span class="tex-font-style-tt">A</span>' if player A wins the game on the given board, and '<span class="tex-font-style-tt">B</span>' if player B will claim the victory. Again, it's guaranteed that there will always be a winner on the given board.</p></div>

## Input

<p>The input consists of the board description given in eight lines, each line contains eight characters. Character '<span class="tex-font-style-tt">B</span>' is used to denote a black pawn, and character '<span class="tex-font-style-tt">W</span>' represents a white pawn. Empty cell is marked with '<span class="tex-font-style-tt">.</span>'. </p><p>It's guaranteed that there will not be white pawns on the first row neither black pawns on the last row.</p>

## Output

<p>Print '<span class="tex-font-style-tt">A</span>' if player A wins the game on the given board, and '<span class="tex-font-style-tt">B</span>' if player B will claim the victory. Again, it's guaranteed that there will always be a winner on the given board.</p>





```input1
........
........
.B....B.
....W...
........
..W.....
........
........

```




```input2
..B.....
..W.....
......B.
........
.....W..
......B.
........
........

```




```output1
A

```




```output2
B

```



## Note

<p>In the first sample player A is able to complete his goal in 3 steps by always moving a pawn initially located at <span class="tex-span">(4, 5)</span>. Player B needs at least 5 steps for any of his pawns to reach the row <span class="tex-span">8</span>. Hence, player A will be the winner.</p>
