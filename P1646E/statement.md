## Description

<div><p>You have a rectangular board of size $n\times m$ ($n$ rows, $m$ columns). The $n$ rows are numbered from $1$ to $n$ from top to bottom, and the $m$ columns are numbered from $1$ to $m$ from left to right. </p><p>The cell at the intersection of row $i$ and column $j$ contains the number $i^j$ ($i$ raised to the power of $j$). For example, if $n=3$ and $m=3$ the board is as follows:</p><center> <img class="tex-graphics" src="file://92zXtC3i.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px"> </center><p>Find the number of distinct integers written on the board.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $m$ ($1\le n,m\le 10^6$)&nbsp;— the number of rows and columns of the board.</p></div><div class="output-specification"><p>Print one integer, the number of distinct integers on the board.</p></div>

## Input

<p>The only line contains two integers $n$ and $m$ ($1\le n,m\le 10^6$)&nbsp;— the number of rows and columns of the board.</p>

## Output

<p>Print one integer, the number of distinct integers on the board.</p>





```input1
3 3
```




```input2
2 4
```




```input3
4 2
```




```output1
7
```




```output2
5
```




```output3
6
```



## Note

<p>The statement shows the board for the first test case. In this case there are $7$ distinct integers: $1$, $2$, $3$, $4$, $8$, $9$, and $27$.</p><p>In the second test case, the board is as follows:</p><center> <img class="tex-graphics" src="file://zTpnoh8w.png" style="max-width: 100.0%;max-height: 100.0%;" width="252px"> </center><p>There are $5$ distinct numbers: $1$, $2$, $4$, $8$ and $16$.</p><p>In the third test case, the board is as follows:</p><center> <img class="tex-graphics" height="252px" src="file://zVP7JSEt.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There are $6$ distinct numbers: $1$, $2$, $3$, $4$, $9$ and $16$.</p>
