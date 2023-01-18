## Description

<div><p>Nash designed an interesting yet simple board game where a player is simply required to follow instructions written on the cell where the player currently stands. </p><p>This board game is played on the $n\times n$ board. Rows and columns of this board are numbered from $1$ to $n$. The cell on the intersection of the $r$-th row and $c$-th column is denoted by $(r, c)$.</p><p>Some cells on the board are called <span class="tex-font-style-bf">blocked zones</span>. On each cell of the board, there is written one of the following $5$ characters &nbsp;— $U$, $D$, $L$, $R$ or $X$ &nbsp;— instructions for the player. Suppose that the current cell is $(r, c)$. If the character is $R$, the player should move to the right cell $(r, c+1)$, for $L$ the player should move to the left cell $(r, c-1)$, for $U$ the player should move to the top cell $(r-1, c)$, for $D$ the player should move to the bottom cell $(r+1, c)$. Finally, if the character in the cell is $X$, then this cell is the <span class="tex-font-style-bf">blocked zone</span>. The player should remain in this cell (the game for him isn't very interesting from now on).</p><p>It is guaranteed that the characters are written in a way that the player will never have to step outside of the board, no matter at which cell he starts.</p><p>As a player starts from a cell, he moves according to the character in the current cell. The player keeps moving until he lands in a blocked zone. It is also possible that the player will keep moving infinitely long.</p><p>For every of the $n^2$ cells of the board Alice, your friend, wants to know, how will the game go, if the player starts in this cell. For each starting cell of the board, she writes down the cell that the player stops at, or that the player never stops at all. She gives you the information she has written: for each cell $(r, c)$ she wrote: </p><ul> <li> a pair ($x$,$y$), meaning if a player had started at $(r, c)$, he would end up at cell ($x$,$y$). </li><li> or a pair ($-1$,$-1$), meaning if a player had started at $(r, c)$, he would keep moving infinitely long and would never enter the blocked zone. </li></ul><p>It might be possible that Alice is trying to fool you and there's no possible grid that satisfies all the constraints Alice gave you. For the given information Alice provided you, you are required to decipher a possible board, or to determine that such a board doesn't exist. If there exist several different boards that satisfy the provided information, you can find any of them.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($1 \leq n \leq 10^{3}$) &nbsp;— the side of the board.</p><p>The $i$-th of the next $n$ lines of the input contains $2n$ integers $x_1, y_1, x_2, y_2, \dots, x_n, y_n$, where $(x_j, y_j)$ ($1 \leq x_j \leq n, 1 \leq y_j \leq n$, or $(x_j,y_j)=(-1,-1)$) is the pair written by Alice for the cell $(i, j)$. </p></div><div class="output-specification"><p>If there doesn't exist a board satisfying the information that Alice gave you, print a single line containing <span class="tex-font-style-tt">INVALID</span>. </p><p>Otherwise, in the first line print <span class="tex-font-style-tt">VALID</span>. In the $i$-th of the next $n$ lines, print the string of $n$ characters, corresponding to the characters in the $i$-th row of the suitable board you found. Each character of a string can either be $U$, $D$, $L$, $R$ or $X$. If there exist several different boards that satisfy the provided information, you can find any of them.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($1 \leq n \leq 10^{3}$) &nbsp;— the side of the board.</p><p>The $i$-th of the next $n$ lines of the input contains $2n$ integers $x_1, y_1, x_2, y_2, \dots, x_n, y_n$, where $(x_j, y_j)$ ($1 \leq x_j \leq n, 1 \leq y_j \leq n$, or $(x_j,y_j)=(-1,-1)$) is the pair written by Alice for the cell $(i, j)$. </p>

## Output

<p>If there doesn't exist a board satisfying the information that Alice gave you, print a single line containing <span class="tex-font-style-tt">INVALID</span>. </p><p>Otherwise, in the first line print <span class="tex-font-style-tt">VALID</span>. In the $i$-th of the next $n$ lines, print the string of $n$ characters, corresponding to the characters in the $i$-th row of the suitable board you found. Each character of a string can either be $U$, $D$, $L$, $R$ or $X$. If there exist several different boards that satisfy the provided information, you can find any of them.</p>





```input1
2
1 1 1 1
2 2 2 2
```




```input2
3
-1 -1 -1 -1 -1 -1
-1 -1 2 2 -1 -1
-1 -1 -1 -1 -1 -1
```




```output1
VALID
XL
RX
```




```output2
VALID
RRD
UXD
ULL
```



## Note

<p>For the sample test 1 :</p><p>The given grid in output is a valid one. </p><ul> <li> If the player starts at $(1,1)$, he doesn't move any further following $X$ and stops there. </li><li> If the player starts at $(1,2)$, he moves to left following $L$ and stops at $(1,1)$. </li><li> If the player starts at $(2,1)$, he moves to right following $R$ and stops at $(2,2)$. </li><li> If the player starts at $(2,2)$, he doesn't move any further following $X$ and stops there. </li></ul><p>The simulation can be seen below : </p><center> <img class="tex-graphics" src="file://vec2s2P5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the sample test 2 : </p><p>The given grid in output is a valid one, as a player starting at any cell other than the one at center $(2,2)$, keeps moving in an infinitely long cycle and never stops. Had he started at $(2,2)$, he wouldn't have moved further following instruction $X$ .</p><p>The simulation can be seen below : </p><center> <img class="tex-graphics" src="file://dFsqNLgq.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
