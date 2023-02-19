## Description

<div><p>You are given a weighted undirected graph on $n$ vertices along with $q$ triples $(u, v, l)$, where in each triple $u$ and $v$ are vertices and $l$ is a positive integer. An edge $e$ is called <span class="tex-font-style-it">useful</span> if there is at least one triple $(u, v, l)$ and a path (not necessarily simple) with the following properties:</p><ul> <li> $u$ and $v$ are the endpoints of this path, </li><li> $e$ is one of the edges of this path, </li><li> the sum of weights of all edges on this path doesn't exceed $l$. </li></ul><p>Please print the number of useful edges in this graph.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2\leq n\leq 600$, $0\leq m\leq \frac{n(n-1)}2$). </p><p>Each of the following $m$ lines contains three integers $u$, $v$ and $w$ ($1\leq u, v\leq n$, $u\neq v$, $1\leq w\leq 10^9$), denoting an edge connecting vertices $u$ and $v$ and having a weight $w$.</p><p>The following line contains the only integer $q$ ($1\leq q\leq \frac{n(n-1)}2$) denoting the number of triples.</p><p>Each of the following $q$ lines contains three integers $u$, $v$ and $l$ ($1\leq u, v\leq n$, $u\neq v$, $1\leq l\leq 10^9$) denoting a triple $(u, v, l)$.</p><p>It's guaranteed that: </p><ul> <li> the graph doesn't contain loops or multiple edges; </li><li> all pairs $(u, v)$ in the triples are also different. </li></ul></div><div class="output-specification"><p>Print a single integer denoting the number of useful edges in the graph.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2\leq n\leq 600$, $0\leq m\leq \frac{n(n-1)}2$). </p><p>Each of the following $m$ lines contains three integers $u$, $v$ and $w$ ($1\leq u, v\leq n$, $u\neq v$, $1\leq w\leq 10^9$), denoting an edge connecting vertices $u$ and $v$ and having a weight $w$.</p><p>The following line contains the only integer $q$ ($1\leq q\leq \frac{n(n-1)}2$) denoting the number of triples.</p><p>Each of the following $q$ lines contains three integers $u$, $v$ and $l$ ($1\leq u, v\leq n$, $u\neq v$, $1\leq l\leq 10^9$) denoting a triple $(u, v, l)$.</p><p>It's guaranteed that: </p><ul> <li> the graph doesn't contain loops or multiple edges; </li><li> all pairs $(u, v)$ in the triples are also different. </li></ul>

## Output

<p>Print a single integer denoting the number of useful edges in the graph.</p>





```input1
4 6
1 2 1
2 3 1
3 4 1
1 3 3
2 4 3
1 4 5
1
1 4 4
```




```input2
4 2
1 2 10
3 4 10
6
1 2 11
1 3 11
1 4 11
2 3 11
2 4 11
3 4 9
```




```input3
3 2
1 2 1
2 3 2
1
1 2 5
```




```output1
5
```




```output2
1
```




```output3
2
```



## Note

<p>In the first example each edge is useful, except the one of weight $5$.</p><p>In the second example only edge between $1$ and $2$ is useful, because it belongs to the path $1-2$, and $10 \leq 11$. The edge between $3$ and $4$, on the other hand, is not useful.</p><p>In the third example both edges are useful, for there is a path $1-2-3-2$ of length exactly $5$. Please note that the path may pass through a vertex more than once.</p>
