## Description

<div><p>You have an array of integers (initially empty).</p><p>You have to perform $q$ queries. Each query is of one of two types: </p><ul> <li> "$1$ $x$"&nbsp;— add the element $x$ to the end of the array; </li><li> "$2$ $x$ $y$"&nbsp;— replace all occurrences of $x$ in the array with $y$. </li></ul><p>Find the resulting array after performing all the queries.</p></div><div class="input-specification"><p>The first line contains a single integer $q$ ($1 \le q \le 5 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Next $q$ lines contain queries (one per line). Each query is of one of two types: </p><ul> <li> "$1$ $x$" ($1 \le x \le 5 \cdot 10^5$); </li><li> "$2$ $x$ $y$" ($1 \le x, y \le 5 \cdot 10^5$). </li></ul><p>It's guaranteed that there is at least one query of the first type.</p></div><div class="output-specification"><p>In a single line, print $k$ integers&nbsp;— the resulting array after performing all the queries, where $k$ is the number of queries of the first type.</p></div>

## Input

<p>The first line contains a single integer $q$ ($1 \le q \le 5 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Next $q$ lines contain queries (one per line). Each query is of one of two types: </p><ul> <li> "$1$ $x$" ($1 \le x \le 5 \cdot 10^5$); </li><li> "$2$ $x$ $y$" ($1 \le x, y \le 5 \cdot 10^5$). </li></ul><p>It's guaranteed that there is at least one query of the first type.</p>

## Output

<p>In a single line, print $k$ integers&nbsp;— the resulting array after performing all the queries, where $k$ is the number of queries of the first type.</p>





```input1
7
1 3
1 1
2 1 2
1 2
1 1
1 2
2 1 3
```




```input2
4
1 1
1 2
1 1
2 2 2
```




```input3
8
2 1 4
1 1
1 4
1 2
2 2 4
2 4 3
1 2
2 2 7
```




```output1
3 2 2 3 2
```




```output2
1 2 1
```




```output3
1 3 3 7
```



## Note

<p>In the first example, the array changes as follows:</p><p>$[]$ $\rightarrow$ $[3]$ $\rightarrow$ $[3, 1]$ $\rightarrow$ $[3, 2]$ $\rightarrow$ $[3, 2, 2]$ $\rightarrow$ $[3, 2, 2, 1]$ $\rightarrow$ $[3, 2, 2, 1, 2]$ $\rightarrow$ $[3, 2, 2, 3, 2]$.</p><p>In the second example, the array changes as follows:</p><p>$[]$ $\rightarrow$ $[1]$ $\rightarrow$ $[1, 2]$ $\rightarrow$ $[1, 2, 1]$ $\rightarrow$ $[1, 2, 1]$.</p><p>In the third example, the array changes as follows:</p><p>$[]$ $\rightarrow$ $[]$ $\rightarrow$ $[1]$ $\rightarrow$ $[1, 4]$ $\rightarrow$ $[1, 4, 2]$ $\rightarrow$ $[1, 4, 4]$ $\rightarrow$ $[1, 3, 3]$ $\rightarrow$ $[1, 3, 3, 2]$ $\rightarrow$ $[1, 3, 3, 7]$.</p>
