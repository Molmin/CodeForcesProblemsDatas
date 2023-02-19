## Description

<div><p>There is a chess board of size $n \times m$. The rows are numbered from $1$ to $n$, the columns are numbered from $1$ to $m$.</p><p>Let's call a cell <span class="tex-font-style-it">isolated</span> if a knight placed in that cell can't move to any other cell on the board. Recall that a chess knight moves two cells in one direction and one cell in a perpendicular direction: </p><center> <img class="tex-graphics" src="file://8kilVrao.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Find any <span class="tex-font-style-it">isolated</span> cell on the board. If there are no such cells, print any cell on the board.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 64$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains two integers $n$ and $m$ ($1 \le n, m \le 8$)&nbsp;— the number of rows and columns of the board.</p></div><div class="output-specification"><p>For each testcase, print two integers&nbsp;— the row and the column of any <span class="tex-font-style-it">isolated</span> cell on the board. If there are no such cells, print any cell on the board.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 64$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains two integers $n$ and $m$ ($1 \le n, m \le 8$)&nbsp;— the number of rows and columns of the board.</p>

## Output

<p>For each testcase, print two integers&nbsp;— the row and the column of any <span class="tex-font-style-it">isolated</span> cell on the board. If there are no such cells, print any cell on the board.</p>





```input1|2,4
3
1 7
8 8
3 3
```




```output1
1 7
7 2
2 2
```



## Note

<p>In the first testcase, all cells are <span class="tex-font-style-it">isolated</span>. A knight can't move from any cell of the board to any other one. Thus, any cell on board is a correct answer.</p><p>In the second testcase, there are no <span class="tex-font-style-it">isolated</span> cells. On a normal chess board, a knight has at least two moves from any cell. Thus, again, any cell is a correct answer.</p><p>In the third testcase, only the middle cell of the board is <span class="tex-font-style-it">isolated</span>. The knight can move freely around the border of the board, but can't escape the middle.</p>
