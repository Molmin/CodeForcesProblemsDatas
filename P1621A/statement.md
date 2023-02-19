## Description

<div><p>You have an $n \times n$ chessboard and $k$ rooks. Rows of this chessboard are numbered by integers from $1$ to $n$ from top to bottom and columns of this chessboard are numbered by integers from $1$ to $n$ from left to right. The cell $(x, y)$ is the cell on the intersection of row $x$ and collumn $y$ for $1 \leq x \leq n$ and $1 \leq y \leq n$.</p><p>The arrangement of rooks on this board is called <span class="tex-font-style-it">good</span>, if no rook is beaten by another rook.</p><p>A rook beats all the rooks that shares the same row or collumn with it.</p><p>The <span class="tex-font-style-bf">good</span> arrangement of rooks on this board is called <span class="tex-font-style-it">not stable</span>, if it is possible to move one rook to the adjacent cell so arrangement becomes not good. Otherwise, the <span class="tex-font-style-bf">good</span> arrangement is <span class="tex-font-style-it">stable</span>. Here, adjacent cells are the cells <span class="tex-font-style-bf">that share a side</span>.</p><center> <img class="tex-graphics" src="file://jlkxR9As.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Such arrangement of $3$ rooks on the $4 \times 4$ chessboard is good, but it is not stable: the rook from $(1, 1)$ can be moved to the adjacent cell $(2, 1)$ and rooks on cells $(2, 1)$ and $(2, 4)$ will beat each other.</span> </center><p>Please, find any stable arrangement of $k$ rooks on the $n \times n$ chessboard or report that there is no such arrangement.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$, $k$ ($1 \leq k \leq n \leq 40$)&nbsp;— the size of the chessboard and the number of rooks.</p></div><div class="output-specification"><p>If there is a stable arrangement of $k$ rooks on the $n \times n$ chessboard, output $n$ lines of symbols <span class="tex-font-style-tt">.</span> and <span class="tex-font-style-tt">R</span>. The $j$-th symbol of the $i$-th line should be equals <span class="tex-font-style-tt">R</span> if and only if there is a rook on the cell $(i, j)$ in your arrangement.</p><p>If there are multiple solutions, you may output any of them.</p><p>If there is no stable arrangement, output $-1$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$, $k$ ($1 \leq k \leq n \leq 40$)&nbsp;— the size of the chessboard and the number of rooks.</p>

## Output

<p>If there is a stable arrangement of $k$ rooks on the $n \times n$ chessboard, output $n$ lines of symbols <span class="tex-font-style-tt">.</span> and <span class="tex-font-style-tt">R</span>. The $j$-th symbol of the $i$-th line should be equals <span class="tex-font-style-tt">R</span> if and only if there is a rook on the cell $(i, j)$ in your arrangement.</p><p>If there are multiple solutions, you may output any of them.</p><p>If there is no stable arrangement, output $-1$.</p>





```input1|2,4,6
5
3 2
3 3
1 1
5 2
40 33
```




```output1
..R
...
R..
-1
R
.....
R....
.....
....R
.....
-1
```



## Note

<p>In the first test case, you should find stable arrangement of $2$ rooks on the $3 \times 3$ chessboard. Placing them in cells $(3, 1)$ and $(1, 3)$ gives stable arrangement.</p><p>In the second test case it can be shown that it is impossbile to place $3$ rooks on the $3 \times 3$ chessboard to get stable arrangement.</p>
