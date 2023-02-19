## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>ICPC Assiut Community decided to hold a unique chess contest, and you were chosen to control a queen and hunt down the hidden king, while a member of ICPC Assiut Community controls this king.</p><p>You compete on an $8\times8$ chessboard, the rows are numerated from top to bottom, and the columns are numerated left to right, and the cell in row $x$ and column $y$ is denoted as $(x, y)$.</p><p>In one turn you can move the queen to any of the squares on the same horizontal line, vertical line, or any of the diagonals. For example, if the queen was on square ($4$, $5$), you can move to ($q_1$, $5$), ($4$, $q_1$), ($q_1$, $9-q_1$), or ($q_2$, $q_2+1$) where ($1 \le q_1 \le 8$, $q_1 \ne 4$, $1 \le q_2 \le 7$, $q_2 \ne 4$). Note that the queen <span class="tex-font-style-bf">cannot</span> stay on its current cell. </p><center> <img class="tex-graphics" src="file://xmwj1m5U.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center><p>In one turn, the king can move "Right", "Left", "Up", "Down", "Down-Right", "Down-Left", "Up-Left", or "Up-Right" such that he doesn't get out of the board. The king <span class="tex-font-style-bf">cannot</span> move into a cell that is on the same row, column or diagonal with the queen (including the position of the queen itself). For example, if the king was on square ($4$, $5$), he can move to ($4+k_1$, $5+k_2$) where ($-1 \le k_1,k_2 \le 1$, $(k_1, k_2) \ne (0, 0)$). </p><center> <img class="tex-graphics" src="file://NHLy9JwQ.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center><p>At the start of the game, you should place the queen at any location on the board, and this is done once per game. After that the king is secretly placed at any cell different from the queen's location. You do not know the position of the king. Then, the king and the queen take turns with the king moving first. The king moves to one of the possible directions ("Right", "Down", "Up-Left", etc.), and you are only given the direction it moves to. After that, you should move your queen by declaring the square to which your queen will move. The game follows like this until you win the game or run out of moves.</p><p>You win if the king has no valid moves. You lose if after $130$ moves of the queen the king still has valid moves.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 60$)&nbsp;— the number of test cases.</p></div><div><h2>Interaction</h2><p>In each test case, you should print the queen's starting cell immediately. If you placed the queen at the king's cell, you will win immediately.</p><p>After that, you may make at most $130$ moves. Each move is made in the format $x$ $y$, where $x$ and $y$ are two integers ($1 \leq x,y \leq 8$) that denote the new row and column of the queen respectively. Your move should be a valid queen move.</p><p>After the initial queen placement and after each move you will receive a string $s$ that represents the direction of the king's move. It will be one of the following: "<span class="tex-font-style-tt">Right</span>", "<span class="tex-font-style-tt">Left</span>", "<span class="tex-font-style-tt">Up</span>", "<span class="tex-font-style-tt">Down</span>", "<span class="tex-font-style-tt">Down-Right</span>", "<span class="tex-font-style-tt">Down-Left</span>", "<span class="tex-font-style-tt">Up-Left</span>", "<span class="tex-font-style-tt">Up-Right</span>", or "<span class="tex-font-style-tt">Done</span>" if you win the game. You should consider "<span class="tex-font-style-tt">Done</span>" as the end of each test case.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p>If at any point you make an invalid query or try to make more than $130$ queries for each test case, the game will terminate immediately and you will receive a Wrong Answer verdict.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 60$)&nbsp;— the number of test cases.</p>





```input1
1
Left
Right
Done
```




```output1
7 5
7 6
7 7
```



## Note

<p>In the example, the hidden king was at $(8, 8)$ at the start. The game follows like this:</p><center> <img class="tex-graphics" src="file://YBatDCUF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <img class="tex-graphics" src="file://uvNkO1Bf.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
