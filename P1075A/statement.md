## Description

<div><p>On a chessboard with a width of $n$ and a height of $n$, rows are numbered from bottom to top from $1$ to $n$, columns are numbered from left to right from $1$ to $n$. Therefore, for each cell of the chessboard, you can assign the coordinates $(r,c)$, where $r$ is the number of the row, and $c$ is the number of the column.</p><p>The white king has been sitting in a cell with $(1,1)$ coordinates for a thousand years, while the black king has been sitting in a cell with $(n,n)$ coordinates. They would have sat like that further, but suddenly a beautiful coin fell on the cell with coordinates $(x,y)$...</p><p>Each of the monarchs wanted to get it, so they decided to arrange a race according to slightly changed chess rules:</p><p>As in chess, the white king makes the first move, the black king makes the second one, the white king makes the third one, and so on. However, in this problem, <span class="tex-font-style-bf">kings can stand in adjacent cells or even in the same cell at the same time</span>.</p><p>The player who reaches the coin first will win, that is to say, the player who reaches the cell with the coordinates $(x,y)$ first will win.</p><p>Let's recall that the king is such a chess piece that can move one cell in all directions, that is, if the king is in the $(a,b)$ cell, then in one move he can move from $(a,b)$ to the cells $(a + 1,b)$, $(a - 1,b)$, $(a,b + 1)$, $(a,b - 1)$, $(a + 1,b - 1)$, $(a + 1,b + 1)$, $(a - 1,b - 1)$, or $(a - 1,b + 1)$. Going outside of the field is prohibited.</p><p>Determine the color of the king, who will reach the cell with the coordinates $(x,y)$ first, if the white king moves first.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 10^{18}$)&nbsp;— the length of the side of the chess field.</p><p>The second line contains two integers $x$ and $y$ ($1 \le x,y \le n$)&nbsp;— coordinates of the cell, where the coin fell.</p></div><div class="output-specification"><p>In a single line print the answer "<span class="tex-font-style-tt">White</span>" (without quotes), if the white king will win, or "<span class="tex-font-style-tt">Black</span>" (without quotes), if the black king will win.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 10^{18}$)&nbsp;— the length of the side of the chess field.</p><p>The second line contains two integers $x$ and $y$ ($1 \le x,y \le n$)&nbsp;— coordinates of the cell, where the coin fell.</p>

## Output

<p>In a single line print the answer "<span class="tex-font-style-tt">White</span>" (without quotes), if the white king will win, or "<span class="tex-font-style-tt">Black</span>" (without quotes), if the black king will win.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
4
2 3

```




```input2
5
3 5

```




```input3
2
2 2

```




```output1
White
```




```output2
Black
```




```output3
Black
```



## Note

<p>An example of the race from the first sample where both the white king and the black king move optimally:</p><ol><li> The white king moves from the cell $(1,1)$ into the cell $(2,2)$.</li><li> The black king moves form the cell $(4,4)$ into the cell $(3,3)$.</li><li> The white king moves from the cell $(2,2)$ into the cell $(2,3)$. This is cell containing the coin, so the white king wins.</li></ol><center> <img class="tex-graphics" src="file://ChddeWxy.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>An example of the race from the second sample where both the white king and the black king move optimally:</p><ol><li> The white king moves from the cell $(1,1)$ into the cell $(2,2)$.</li><li> The black king moves form the cell $(5,5)$ into the cell $(4,4)$.</li><li> The white king moves from the cell $(2,2)$ into the cell $(3,3)$.</li><li> The black king moves from the cell $(4,4)$ into the cell $(3,5)$. This is the cell, where the coin fell, so the black king wins.</li></ol><center> <img class="tex-graphics" src="file://hatEWjDh.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third example, the coin fell in the starting cell of the black king, so the black king immediately wins.</p><center> <img class="tex-graphics" src="file://YFke1Efs.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
