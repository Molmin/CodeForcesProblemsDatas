## Description

<div><p>You are given an undirected graph with $n$ vertices numbered from $1$ to $n$. Initially there are no edges.</p><p>You are asked to perform some queries on the graph. Let $last$ be the answer to the latest query of the second type, it is set to $0$ before the first such query. Then the queries are the following:</p><ul> <li> $1~x~y$ ($1 \le x, y \le n$, $x \ne y$) — add an undirected edge between the vertices $(x + last - 1)~mod~n + 1$ and $(y + last - 1)~mod~n + 1$ if it doesn't exist yet, otherwise remove it; </li><li> $2~x~y$ ($1 \le x, y \le n$, $x \ne y$) — check if there exists a path between the vertices $(x + last - 1)~mod~n + 1$ and $(y + last - 1)~mod~n + 1$, which goes only through currently existing edges, and set $last$ to $1$ if so and $0$ otherwise. </li></ul><p>Good luck!</p></div><div class="input-specification"><p>The first line contains two integer numbers $n$ and $m$ ($2 \le n, m \le 2 \cdot 10^5$) — the number of vertices and the number of queries, respectively.</p><p>Each of the following $m$ lines contains a query of one of two aforementioned types. It is guaranteed that there is at least one query of the second type.</p></div><div class="output-specification"><p>Print a string, consisting of characters '0' and '1'. The $i$-th character should be the answer to the $i$-th query of the second type. Therefore the length of the string should be equal to the number of queries of the second type.</p></div>

## Input

<p>The first line contains two integer numbers $n$ and $m$ ($2 \le n, m \le 2 \cdot 10^5$) — the number of vertices and the number of queries, respectively.</p><p>Each of the following $m$ lines contains a query of one of two aforementioned types. It is guaranteed that there is at least one query of the second type.</p>

## Output

<p>Print a string, consisting of characters '0' and '1'. The $i$-th character should be the answer to the $i$-th query of the second type. Therefore the length of the string should be equal to the number of queries of the second type.</p>





```input1
5 9
1 1 2
1 1 3
2 3 2
1 2 4
2 3 4
1 2 4
2 3 4
1 1 3
2 4 3
```




```input2
3 9
1 1 2
1 2 3
1 3 1
2 1 3
1 3 2
2 2 3
1 1 2
2 1 2
2 1 2
```




```output1
1010
```




```output2
1101
```



## Note

<p>The converted queries in the first example are:</p><ul> <li> 1 1 2 </li><li> 1 1 3 </li><li> 2 3 2 </li><li> 1 3 5 </li><li> 2 4 5 </li><li> 1 2 4 </li><li> 2 3 4 </li><li> 1 2 4 </li><li> 2 5 4 </li></ul><p>The converted queries in the second example are:</p><ul> <li> 1 1 2 </li><li> 1 2 3 </li><li> 1 3 1 </li><li> 2 1 3 </li><li> 1 1 3 </li><li> 2 3 1 </li><li> 1 2 3 </li><li> 2 2 3 </li><li> 2 1 2 </li></ul>
