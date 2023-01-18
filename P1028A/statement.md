## Description

<div><p>Consider a table of size $n \times m$, initially fully white. Rows are numbered $1$ through $n$ from top to bottom, columns $1$ through $m$ from left to right. Some square inside the table with <span class="tex-font-style-bf">odd</span> side length was painted black. Find the center of this square.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 115$) — the number of rows and the number of columns in the table.</p><p>The $i$-th of the next $n$ lines contains a string of $m$ characters $s_{i1} s_{i2} \ldots s_{im}$ ($s_{ij}$ is '<span class="tex-font-style-tt">W</span>' for white cells and '<span class="tex-font-style-tt">B</span>' for black cells), describing the $i$-th row of the table.</p></div><div class="output-specification"><p>Output two integers $r$ and $c$ ($1 \le r \le n$, $1 \le c \le m$) separated by a space — the row and column numbers of the center of the black square.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 115$) — the number of rows and the number of columns in the table.</p><p>The $i$-th of the next $n$ lines contains a string of $m$ characters $s_{i1} s_{i2} \ldots s_{im}$ ($s_{ij}$ is '<span class="tex-font-style-tt">W</span>' for white cells and '<span class="tex-font-style-tt">B</span>' for black cells), describing the $i$-th row of the table.</p>

## Output

<p>Output two integers $r$ and $c$ ($1 \le r \le n$, $1 \le c \le m$) separated by a space — the row and column numbers of the center of the black square.</p>





```input1
5 6
WWBBBW
WWBBBW
WWBBBW
WWWWWW
WWWWWW

```




```input2
3 3
WWW
BWW
WWW

```




```output1
2 4

```




```output2
2 1

```


