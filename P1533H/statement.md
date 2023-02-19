## Description

<div><p>You are given matrix $s$ that contains $n$ rows and $m$ columns. Each element of a matrix is one of the $5$ first Latin letters (in upper case).</p><p>For each $k$ ($1 \le k \le 5$) calculate the number of submatrices that contain exactly $k$ different letters. Recall that a submatrix of matrix $s$ is a matrix that can be obtained from $s$ after removing several (possibly zero) first rows, several (possibly zero) last rows, several (possibly zero) first columns, and several (possibly zero) last columns. If some submatrix can be obtained from $s$ in two or more ways, you have to count this submatrix the corresponding number of times.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 800$).</p><p>Then $n$ lines follow, each containing the string $s_i$ ($|s_i| = m$)&nbsp;— $i$-th row of the matrix. </p></div><div class="output-specification"><p>For each $k$ ($1 \le k \le 5$) print one integer&nbsp;— the number of submatrices that contain exactly $k$ different letters.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 800$).</p><p>Then $n$ lines follow, each containing the string $s_i$ ($|s_i| = m$)&nbsp;— $i$-th row of the matrix. </p>

## Output

<p>For each $k$ ($1 \le k \le 5$) print one integer&nbsp;— the number of submatrices that contain exactly $k$ different letters.</p>





```input1
2 3
ABB
ABA
```




```input2
6 6
EDCECE
EDDCEB
ACCECC
BAEEDC
DDDDEC
DDAEAD
```




```input3
3 10
AEAAEEEEEC
CEEAAEEEEE
CEEEEAACAA
```




```output1
9 9 0 0 0
```




```output2
56 94 131 103 57
```




```output3
78 153 99 0 0
```


