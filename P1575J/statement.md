## Description

<div><p>Mr. Chanek has a new game called Dropping Balls. Initially, Mr. Chanek has a grid $a$ of size $n \times m$</p><p>Each cell $(x,y)$ contains an integer $a_{x,y}$ denoting the direction of how the ball will move.</p><ul> <li> $a_{x,y}=1$ — the ball will move to the right (the next cell is $(x, y + 1)$); </li><li> $a_{x,y}=2$ — the ball will move to the bottom (the next cell is $(x + 1, y)$); </li><li> $a_{x,y}=3$ — the ball will move to the left (the next cell is $(x, y - 1)$). </li></ul><p>Every time a ball leaves a cell $(x,y)$, the integer $a_{x,y}$ will change to $2$. Mr. Chanek will drop $k$ balls sequentially, each starting from the first row, and on the $c_1, c_2, \dots, c_k$-th ($1 \leq c_i \leq m$) columns.</p><p>Determine in which column each ball will end up in (<span class="tex-font-style-bf">position of the ball after leaving the grid</span>).</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, and $k$ ($1 \leq n, m \leq 1000$, $1 \leq k \leq 10^5$) — the size of the grid and the number of balls dropped by Mr. Chanek.</p><p>The $i$-th of the next $n$ lines contains $m$ integers $a_{i,1},a_{i,2},\ldots,a_{i,m}$ ($1 \leq a_{i,j} \leq 3$). It will satisfy $a_{i, 1} \ne 3$ and $a_{i, m} \ne 1$.</p><p>The next line contains $k$ integers $c_1, c_2, \ldots, c_k$ ($1 \leq c_i \leq m$) — the balls' column positions dropped by Mr. Chanek sequentially.</p></div><div class="output-specification"><p>Output $k$ integers — the $i$-th integer denoting the column where the $i$-th ball will end.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, and $k$ ($1 \leq n, m \leq 1000$, $1 \leq k \leq 10^5$) — the size of the grid and the number of balls dropped by Mr. Chanek.</p><p>The $i$-th of the next $n$ lines contains $m$ integers $a_{i,1},a_{i,2},\ldots,a_{i,m}$ ($1 \leq a_{i,j} \leq 3$). It will satisfy $a_{i, 1} \ne 3$ and $a_{i, m} \ne 1$.</p><p>The next line contains $k$ integers $c_1, c_2, \ldots, c_k$ ($1 \leq c_i \leq m$) — the balls' column positions dropped by Mr. Chanek sequentially.</p>

## Output

<p>Output $k$ integers — the $i$-th integer denoting the column where the $i$-th ball will end.</p>





```input1
5 5 3
1 2 3 3 3
2 2 2 2 2
2 2 2 2 2
2 2 2 2 2
2 2 2 2 2
1 2 1
```




```input2
1 2 2
1 3
1 2
```




```output1
2 2 1
```




```output2
1 2
```



## Note

<p>In the first example, the first ball will drop as follows. Note that the cell $(1, 1)$ will change direction to the bottom direction.</p><center> <img class="tex-graphics" src="file://XiQyV9f1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The second and third balls will drop as follows. </p><center> <img class="tex-graphics" src="file://XHLgXNcp.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p><span class="tex-font-style-bf">All balls will be dropped from the first row and on the $c_1, c_2, \dots, c_k$-th columns respectively. A ball will stop dropping once it leaves the grid</span>.</p>
