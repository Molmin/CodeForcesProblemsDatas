## Description

<div><p>Boboniu has a <span class="tex-font-style-bf">directed</span> graph with $n$ vertices and $m$ edges.</p><p>The out-degree of each vertex is at most $k$.</p><p>Each edge has an integer weight between $1$ and $m$. No two edges have equal weights.</p><p>Boboniu likes to walk on the graph with some specific rules, which is represented by a tuple $(c_1,c_2,\ldots,c_k)$. If he now stands on a vertex $u$ with out-degree $i$, then he will go to the next vertex by the edge with the $c_i$-th $(1\le c_i\le i)$ smallest weight among all edges outgoing from $u$.</p><p>Now Boboniu asks you to calculate the number of tuples $(c_1,c_2,\ldots,c_k)$ such that</p><ul> <li> $1\le c_i\le i$ for all $i$ ($1\le i\le k$). </li><li> Starting from any vertex $u$, it is possible to go back to $u$ in finite time by walking on the graph under the described rules. </li></ul></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $k$ ($2\le n\le 2\cdot 10^5$, $2\le m\le \min(2\cdot 10^5,n(n-1) )$, $1\le k\le 9$).</p><p>Each of the next $m$ lines contains three integers $u$, $v$ and $w$ $(1\le u,v\le n,u\ne v,1\le w\le m)$, denoting an edge from $u$ to $v$ with weight $w$. It is guaranteed that there are no self-loops or multiple edges and each vertex has at least one edge starting from itself.</p><p>It is guaranteed that the out-degree of each vertex is at most $k$ and no two edges have equal weight.</p></div><div class="output-specification"><p>Print one integer: the number of tuples.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $k$ ($2\le n\le 2\cdot 10^5$, $2\le m\le \min(2\cdot 10^5,n(n-1) )$, $1\le k\le 9$).</p><p>Each of the next $m$ lines contains three integers $u$, $v$ and $w$ $(1\le u,v\le n,u\ne v,1\le w\le m)$, denoting an edge from $u$ to $v$ with weight $w$. It is guaranteed that there are no self-loops or multiple edges and each vertex has at least one edge starting from itself.</p><p>It is guaranteed that the out-degree of each vertex is at most $k$ and no two edges have equal weight.</p>

## Output

<p>Print one integer: the number of tuples.</p>





```input1
4 6 3
4 2 1
1 2 2
2 4 3
4 1 4
4 3 5
3 1 6
```




```input2
5 5 1
1 4 1
5 1 2
2 5 3
4 3 4
3 2 5
```




```input3
6 13 4
3 5 1
2 5 2
6 3 3
1 4 4
2 6 5
5 3 6
4 1 7
4 3 8
5 2 9
4 2 10
2 1 11
6 1 12
4 6 13
```




```output1
2
```




```output2
1
```




```output3
1
```



## Note

<p>For the first example, there are two tuples: $(1,1,3)$ and $(1,2,3)$. The blue edges in the picture denote the $c_i$-th smallest edges for each vertex, which Boboniu chooses to go through.</p><center> <img class="tex-graphics" src="file://C7v6qf7c.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the third example, there's only one tuple: $(1,2,2,2)$.</p><center> <img class="tex-graphics" src="file://x2RYsueo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The <span class="tex-font-style-it">out-degree</span> of vertex $u$ means the number of edges outgoing from $u$.</p>
