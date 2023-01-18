## Description

<div><p>There is given an integer $k$ and a grid $2^k \times 2^k$ with some numbers written in its cells, cell $(i, j)$ initially contains number $a_{ij}$. Grid is considered to be a torus, that is, the cell to the right of $(i, 2^k)$ is $(i, 1)$, the cell below the $(2^k, i)$ is $(1, i)$ There is also given a lattice figure $F$, consisting of $t$ cells, where $t$ is <span class="tex-font-style-bf">odd</span>. $F$ doesn't have to be connected.</p><p>We can perform the following operation: place $F$ at some position on the grid. (Only translations are allowed, rotations and reflections are prohibited). Now choose any nonnegative integer $p$. After that, for each cell $(i, j)$, covered by $F$, replace $a_{ij}$ by $a_{ij}\oplus p$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>More formally, let $F$ be given by cells $(x_1, y_1), (x_2, y_2), \dots, (x_t, y_t)$. Then you can do the following operation: choose any $x, y$ with $1\le x, y \le 2^k$, any nonnegative integer $p$, and for every $i$ from $1$ to $n$ replace number in the cell $(((x + x_i - 1)\bmod 2^k) + 1, ((y + y_i - 1)\bmod 2^k) + 1)$ with $a_{((x + x_i - 1)\bmod 2^k) + 1, ((y + y_i - 1)\bmod 2^k) + 1}\oplus p$.</p><p>Our goal is to make all the numbers equal to $0$. Can we achieve it? If we can, find the smallest number of operations in which it is possible to do this.</p></div><div class="input-specification"><p>The first line contains a single integer $k$ ($1 \le k \le 9$).</p><p>The $i$-th of the next $2^k$ lines contains $2^k$ integers $a_{i1}, a_{i2}, \dots, a_{i2^k}$ ($0 \le a_{ij} &lt; 2^{60}$)&nbsp;— initial values in the $i$-th row of the grid.</p><p>The next line contains a single integer $t$ ($1\le t \le \min(99, 4^k)$, $t$ is odd)&nbsp;— number of cells of figure.</p><p>$i$-th of next $t$ lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 2^k$), describing the position of the $i$-th cell of the figure.</p><p>It is guaranteed that all cells are different, but <span class="tex-font-style-bf">it is not guaranteed that the figure is connected</span>. </p></div><div class="output-specification"><p>If it is impossible to make all numbers in the grid equal to $0$ with these operations, output $-1$.</p><p>Otherwise, output a single integer&nbsp;— the minimal number of operations needed to do this. It can be shown that if it is possible to make all numbers equal $0$, it is possible to do so in less than $10^{18}$ operations.</p></div>

## Input

<p>The first line contains a single integer $k$ ($1 \le k \le 9$).</p><p>The $i$-th of the next $2^k$ lines contains $2^k$ integers $a_{i1}, a_{i2}, \dots, a_{i2^k}$ ($0 \le a_{ij} &lt; 2^{60}$)&nbsp;— initial values in the $i$-th row of the grid.</p><p>The next line contains a single integer $t$ ($1\le t \le \min(99, 4^k)$, $t$ is odd)&nbsp;— number of cells of figure.</p><p>$i$-th of next $t$ lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 2^k$), describing the position of the $i$-th cell of the figure.</p><p>It is guaranteed that all cells are different, but <span class="tex-font-style-bf">it is not guaranteed that the figure is connected</span>. </p>

## Output

<p>If it is impossible to make all numbers in the grid equal to $0$ with these operations, output $-1$.</p><p>Otherwise, output a single integer&nbsp;— the minimal number of operations needed to do this. It can be shown that if it is possible to make all numbers equal $0$, it is possible to do so in less than $10^{18}$ operations.</p>





```input1
2
5 5 5 5
2 6 2 3
0 0 2 0
0 0 0 0
5
1 1
1 2
1 3
1 4
2 4
```




```output1
3
```



## Note

<p>The figure and the operations for the example are shown above:</p><center> <img class="tex-graphics" src="file://8xI0s5qJ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
