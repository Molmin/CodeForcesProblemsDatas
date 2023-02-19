## Description

<div><p>You are given a matrix $a$, consisting of $3$ rows and $n$ columns. Each cell of the matrix is either free or taken.</p><p>A free cell $y$ is reachable from a free cell $x$ if at least one of these conditions hold: </p><ul> <li> $x$ and $y$ share a side; </li><li> there exists a free cell $z$ such that $z$ is reachable from $x$ and $y$ is reachable from $z$. </li></ul><p>A connected component is a set of free cells of the matrix such that all cells in it are reachable from one another, but adding any other free cell to the set violates this rule.</p><p>You are asked $q$ queries about the matrix. Each query is the following: </p><ul> <li> $l$ $r$&nbsp;— count the number of connected components of the matrix, consisting of columns from $l$ to $r$ of the matrix $a$, inclusive. </li></ul><p>Print the answers to all queries.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 5 \cdot 10^5$)&nbsp;— the number of columns of matrix $a$.</p><p>The $i$-th of the next three lines contains a description of the $i$-th row of the matrix $a$&nbsp;— a string, consisting of $n$ characters. Each character is either $1$ (denoting a free cell) or $0$ (denoting a taken cell).</p><p>The next line contains an integer $q$ ($1 \le q \le 3 \cdot 10^5$)&nbsp;— the number of queries.</p><p>The $j$-th of the next $q$ lines contains two integers $l_j$ and $r_j$ ($1 \le l_j \le r_j \le n$)&nbsp;— the description of the $j$-th query.</p></div><div class="output-specification"><p>Print $q$ integers&nbsp;— the $j$-th value should be equal to the number of the connected components of the matrix, consisting of columns from $l_j$ to $r_j$ of the matrix $a$, inclusive.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 5 \cdot 10^5$)&nbsp;— the number of columns of matrix $a$.</p><p>The $i$-th of the next three lines contains a description of the $i$-th row of the matrix $a$&nbsp;— a string, consisting of $n$ characters. Each character is either $1$ (denoting a free cell) or $0$ (denoting a taken cell).</p><p>The next line contains an integer $q$ ($1 \le q \le 3 \cdot 10^5$)&nbsp;— the number of queries.</p><p>The $j$-th of the next $q$ lines contains two integers $l_j$ and $r_j$ ($1 \le l_j \le r_j \le n$)&nbsp;— the description of the $j$-th query.</p>

## Output

<p>Print $q$ integers&nbsp;— the $j$-th value should be equal to the number of the connected components of the matrix, consisting of columns from $l_j$ to $r_j$ of the matrix $a$, inclusive.</p>





```input1
12
100101011101
110110010110
010001011101
8
1 12
1 1
1 2
9 9
8 11
9 12
11 12
4 6
```




```output1
7
1
1
2
1
3
3
3
```


