## Description

<div><p>You are given an undirected weighted graph, consisting of $n$ vertices and $m$ edges.</p><p>Some queries happen with this graph:</p><ul> <li> Delete an existing edge from the graph. </li><li> Add a non-existing edge to the graph. </li></ul><p>At the beginning and after each query, you should find four <span class="tex-font-style-bf">different</span> vertices $a$, $b$, $c$, $d$ such that there exists a path between $a$ and $b$, there exists a path between $c$ and $d$, and the sum of lengths of two shortest paths from $a$ to $b$ and from $c$ to $d$ is minimal. The answer to the query is the sum of the lengths of these two shortest paths. The length of the path is equal to the sum of weights of edges in this path.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ $(4 \le n, m \le 10^5)$&nbsp;— the number of vertices and edges in the graph respectively.</p><p>Each of the next $m$ lines contain three integers $v$, $u$, $w$ ($1 \le v, u \le n, v \neq u$, $1 \le w \le 10^9$)&nbsp;— this triple means that there is an edge between vertices $v$ and $u$ with weight $w$.</p><p>The next line contains a single integer $q$ $(0 \le q \le 10^5)$&nbsp;— the number of queries.</p><p>The next $q$ lines contain the queries of two types:</p><ul> <li> $0$ $v$ $u$&nbsp;— this query means deleting an edge between $v$ and $u$ $(1 \le v, u \le n, v \neq u)$. It is guaranteed that such edge exists in the graph. </li><li> $1$ $v$ $u$ $w$&nbsp;— this query means adding an edge between vertices $v$ and $u$ with weight $w$ ($1 \le v, u \le n, v \neq u$, $1 \le w \le 10^9$). It is guaranteed that there was no such edge in the graph. </li></ul><p>It is guaranteed that the initial graph does not contain multiple edges.</p><p>At the beginning and after each query, the graph <span class="tex-font-style-bf">doesn't need</span> to be connected.</p><p>It is guaranteed that at each moment the number of edges <span class="tex-font-style-bf">will be at least $4$</span>. It can be proven, that at each moment there exist some four vertices $a$, $b$, $c$, $d$ such that there exists a path between vertices $a$ and $b$, and there exists a path between vertices $c$ and $d$.</p></div><div class="output-specification"><p>Print $q + 1$ integers&nbsp;— the minimal sum of lengths of shortest paths between chosen pairs of vertices before the queries and after each of them.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ $(4 \le n, m \le 10^5)$&nbsp;— the number of vertices and edges in the graph respectively.</p><p>Each of the next $m$ lines contain three integers $v$, $u$, $w$ ($1 \le v, u \le n, v \neq u$, $1 \le w \le 10^9$)&nbsp;— this triple means that there is an edge between vertices $v$ and $u$ with weight $w$.</p><p>The next line contains a single integer $q$ $(0 \le q \le 10^5)$&nbsp;— the number of queries.</p><p>The next $q$ lines contain the queries of two types:</p><ul> <li> $0$ $v$ $u$&nbsp;— this query means deleting an edge between $v$ and $u$ $(1 \le v, u \le n, v \neq u)$. It is guaranteed that such edge exists in the graph. </li><li> $1$ $v$ $u$ $w$&nbsp;— this query means adding an edge between vertices $v$ and $u$ with weight $w$ ($1 \le v, u \le n, v \neq u$, $1 \le w \le 10^9$). It is guaranteed that there was no such edge in the graph. </li></ul><p>It is guaranteed that the initial graph does not contain multiple edges.</p><p>At the beginning and after each query, the graph <span class="tex-font-style-bf">doesn't need</span> to be connected.</p><p>It is guaranteed that at each moment the number of edges <span class="tex-font-style-bf">will be at least $4$</span>. It can be proven, that at each moment there exist some four vertices $a$, $b$, $c$, $d$ such that there exists a path between vertices $a$ and $b$, and there exists a path between vertices $c$ and $d$.</p>

## Output

<p>Print $q + 1$ integers&nbsp;— the minimal sum of lengths of shortest paths between chosen pairs of vertices before the queries and after each of them.</p>





```input1
6 6
1 3 6
4 3 1
1 4 1
2 6 4
2 4 2
5 4 3
4
1 2 5 2
0 1 4
0 3 4
1 6 1 3
```




```output1
4
3
3
7
5
```



## Note

<p>Before the queries you can choose vertices $(a, b) = (3, 2)$ and $(c, d) = (1, 4)$. The sum of lengths of two shortest paths is $3 + 1 = 4$.</p><p>After the first query you can choose vertices $(a, b) = (2, 5)$ and $(c, d) = (1, 4)$. The sum of lengths of two shortest paths is $2 + 1 = 3$.</p><p>After the second query you can choose vertices $(a, b) = (3, 4)$ and $(c, d) = (2, 5)$. The sum of lengths of two shortest paths is $1 + 2 = 3$.</p><p>After the third query, you can choose vertices $(a, b) = (2, 6)$ and $(c, d) = (4, 5)$. The sum of lengths of two shortest paths is $4 + 3 = 7$.</p><p>After the last query you can choose vertices $(a, b) = (1, 6)$ and $(c, d) = (2, 5)$. The sum of lengths of two shortest paths is $3 + 2 = 5$.</p>
