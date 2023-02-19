## Description

<div><p>Koa the Koala has a <span class="tex-font-style-bf">directed</span> graph $G$ with $n$ nodes and $m$ edges. Each edge has a capacity associated with it. Exactly $k$ edges of the graph, numbered from $1$ to $k$, are special, such edges initially have a capacity equal to $0$.</p><p>Koa asks you $q$ queries. In each query she gives you $k$ integers $w_1, w_2, \ldots, w_k$. This means that capacity of the $i$-th special edge becomes $w_i$ (and other capacities remain the same).</p><p>Koa wonders: what is the <a href="https://en.wikipedia.org/wiki/Maximum_flow_problem#Definition">maximum flow</a> that goes from node $1$ to node $n$ after each such query?</p><p>Help her!</p></div><div class="input-specification"><p>The first line of the input contains four integers $n$, $m$, $k$, $q$ ($2 \le n \le 10^4$, $1 \le m \le 10^4$, $1 \le k \le \min(10, m)$, $1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of nodes, the number of edges, the number of special edges and the number of queries.</p><p>Each of the next $m$ lines contains three integers $u$, $v$, $w$ ($1 \le u, v \le n$; $0 \le w \le 25$)&nbsp;— the description of a directed edge from node $u$ to node $v$ with capacity $w$.</p><p>Edges are numbered starting from $1$ in the same order they are listed in the input. The first $k$ edges are the special edges. It is guaranteed that $w_i = 0$ for all $i$ with $1 \le i \le k$.</p><p>Each of the next $q$ lines contains $k$ integers $w_1, w_2, \ldots, w_k$ ($0 \le w_i \le 25$) &nbsp;— the description of the query. $w_i$ denotes the capacity of $i$-th edge.</p></div><div class="output-specification"><p>For the $i$-th query, print one integer $res_i$ &nbsp;— the maximum flow that can be obtained from node $1$ to node $n$ given the $i$-th query's special edge weights.</p></div>

## Input

<p>The first line of the input contains four integers $n$, $m$, $k$, $q$ ($2 \le n \le 10^4$, $1 \le m \le 10^4$, $1 \le k \le \min(10, m)$, $1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of nodes, the number of edges, the number of special edges and the number of queries.</p><p>Each of the next $m$ lines contains three integers $u$, $v$, $w$ ($1 \le u, v \le n$; $0 \le w \le 25$)&nbsp;— the description of a directed edge from node $u$ to node $v$ with capacity $w$.</p><p>Edges are numbered starting from $1$ in the same order they are listed in the input. The first $k$ edges are the special edges. It is guaranteed that $w_i = 0$ for all $i$ with $1 \le i \le k$.</p><p>Each of the next $q$ lines contains $k$ integers $w_1, w_2, \ldots, w_k$ ($0 \le w_i \le 25$) &nbsp;— the description of the query. $w_i$ denotes the capacity of $i$-th edge.</p>

## Output

<p>For the $i$-th query, print one integer $res_i$ &nbsp;— the maximum flow that can be obtained from node $1$ to node $n$ given the $i$-th query's special edge weights.</p>





```input1
2 1 1 3
1 2 0
0
1
2
```




```input2
4 4 2 5
1 2 0
2 3 0
2 4 5
3 4 2
0 0
1 10
10 0
7 1
7 2
```




```output1
0
1
2
```




```output2
0
1
5
6
7
```



## Note

<p>For the second sample, the following images correspond to the first two queries (from left to right respectively). For each edge there is a pair <span class="tex-font-style-tt">flow/capacity</span> denoting flow pushed through the edge and edge's capacity. The special edges are colored in red.</p><center> <img class="tex-graphics" src="file://7rl6qqAK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>As you can see in first query maximum flow from node $1$ to node $4$ equals $0$ and in second query equals $1$.</p>
