## Description

<div><p>You are given $n$ arrays that can have different sizes. You also have a table with $w$ columns and $n$ rows. The $i$-th array is placed horizontally in the $i$-th row. You can slide each array within its row as long as it occupies several consecutive cells and lies completely inside the table.</p><p>You need to find the maximum sum of the integers in the $j$-th column for each $j$ from $1$ to $w$ independently.</p><center> <img class="tex-graphics" src="file://66ybU93V.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Optimal placements for columns $1$, $2$ and $3$ are shown on the pictures from left to right.</span> </center><p>Note that you can exclude any array out of a column provided it remains in the window. In this case its value is considered to be zero.</p></div><div class="input-specification"><p>The first line contains two integers $n$ ($1 \le n \le 10^{6}$) and $w$ ($1 \le w \le 10^{6}$)&nbsp;— the number of arrays and the width of the table.</p><p>Each of the next $n$ lines consists of an integer $l_{i}$ ($1 \le l_{i} \le w$), the length of the $i$-th array, followed by $l_{i}$ integers $a_{i1}, a_{i2}, \ldots, a_{il_i}$ ($-10^{9} \le a_{ij} \le 10^{9}$)&nbsp;— the elements of the array.</p><p>The total length of the arrays does no exceed $10^{6}$.</p></div><div class="output-specification"><p>Print $w$ integers, the $i$-th of them should be the maximum sum for column $i$.</p></div>

## Input

<p>The first line contains two integers $n$ ($1 \le n \le 10^{6}$) and $w$ ($1 \le w \le 10^{6}$)&nbsp;— the number of arrays and the width of the table.</p><p>Each of the next $n$ lines consists of an integer $l_{i}$ ($1 \le l_{i} \le w$), the length of the $i$-th array, followed by $l_{i}$ integers $a_{i1}, a_{i2}, \ldots, a_{il_i}$ ($-10^{9} \le a_{ij} \le 10^{9}$)&nbsp;— the elements of the array.</p><p>The total length of the arrays does no exceed $10^{6}$.</p>

## Output

<p>Print $w$ integers, the $i$-th of them should be the maximum sum for column $i$.</p>





```input1
3 3
3 2 4 8
2 2 5
2 6 3
```




```input2
2 2
2 7 8
1 -8
```




```output1
10 15 16
```




```output2
7 8
```



## Note

<p>Illustration for the first example is in the statement.</p>
