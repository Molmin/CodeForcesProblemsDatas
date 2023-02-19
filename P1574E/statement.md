## Description

<div><p>A matrix of size $n \times m$, such that each cell of it contains either $0$ or $1$, is considered <span class="tex-font-style-it">beautiful</span> if the sum in every contiguous submatrix of size $2 \times 2$ is exactly $2$, i. e. every "square" of size $2 \times 2$ contains exactly two $1$'s and exactly two $0$'s.</p><p>You are given a matrix of size $n \times m$. Initially each cell of this matrix is empty. Let's denote the cell on the intersection of the $x$-th row and the $y$-th column as $(x, y)$. You have to process the queries of three types:</p><ul> <li> $x$ $y$ $-1$ — clear the cell $(x, y)$, if there was a number in it; </li><li> $x$ $y$ $0$ — write the number $0$ in the cell $(x, y)$, <span class="tex-font-style-bf">overwriting the number that was there previously (if any)</span>; </li><li> $x$ $y$ $1$ — write the number $1$ in the cell $(x, y)$, <span class="tex-font-style-bf">overwriting the number that was there previously (if any)</span>. </li></ul><p>After each query, print the number of ways to fill the empty cells of the matrix so that the resulting matrix is <span class="tex-font-style-it">beautiful</span>. Since the answers can be large, print them modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $k$ ($2 \le n, m \le 10^6$; $1 \le k \le 3 \cdot 10^5$) — the number of rows in the matrix, the number of columns, and the number of queries, respectively.</p><p>Then $k$ lines follow, the $i$-th of them contains three integers $x_i$, $y_i$, $t_i$ ($1 \le x_i \le n$; $1 \le y_i \le m$; $-1 \le t_i \le 1$) — the parameters for the $i$-th query.</p></div><div class="output-specification"><p>For each query, print one integer — the number of ways to fill the empty cells of the matrix after the respective query, taken modulo $998244353$.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $k$ ($2 \le n, m \le 10^6$; $1 \le k \le 3 \cdot 10^5$) — the number of rows in the matrix, the number of columns, and the number of queries, respectively.</p><p>Then $k$ lines follow, the $i$-th of them contains three integers $x_i$, $y_i$, $t_i$ ($1 \le x_i \le n$; $1 \le y_i \le m$; $-1 \le t_i \le 1$) — the parameters for the $i$-th query.</p>

## Output

<p>For each query, print one integer — the number of ways to fill the empty cells of the matrix after the respective query, taken modulo $998244353$.</p>





```input1
2 2 7
1 1 1
1 2 1
2 1 1
1 1 0
1 2 -1
2 1 -1
1 1 -1
```




```output1
3
1
0
1
2
3
6
```


