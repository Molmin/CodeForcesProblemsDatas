## Description

<div><p>Pak Chanek has a tree called the key tree. This tree consists of $N$ vertices and $N-1$ edges. The edges of the tree are numbered from $1$ to $N-1$ with edge $i$ connecting vertices $U_i$ and $V_i$. Initially, each edge of the key tree does not have a weight.</p><p>Formally, a path with length $k$ in a graph is a sequence $[v_1, e_1, v_2, e_2, v_3, e_3, \ldots, v_k, e_k, v_{k+1}]$ such that: </p><ul> <li> For each $i$, $v_i$ is a vertex and $e_i$ is an edge. </li><li> For each $i$, $e_i$ connects vertices $v_i$ and $v_{i+1}$. </li></ul><p>A circuit is a path that starts and ends on the same vertex.</p><p>A path in a graph is said to be simple if and only if the path does not use the same edge more than once. Note that a simple path can use the same vertex more than once.</p><p>The cost of a simple path in a weighted graph is defined as the <span class="tex-font-style-bf">maximum weight</span> of all edges it traverses.</p><p>Count the number of distinct undirected weighted graphs that satisfy the following conditions: </p><ul> <li> The graph has $N$ vertices and $2N-2$ edges. </li><li> For each pair of different vertices $(x, y)$, there exists a simple circuit that goes through vertices $x$ and $y$ in the graph. </li><li> The weight of each edge in the graph is an integer between $1$ and $2N-2$ inclusive. Each edge has <span class="tex-font-style-bf">distinct</span> weights. </li><li> The graph is formed in a way such that there is a way to assign a weight $W_i$ to each edge $i$ in the key tree that satisfies the following conditions: <ul> <li> For each pair of edges $(i, j)$, if $i&lt;j$, then $W_i&lt;W_j$. </li><li> For each pair of different vertex indices $(x, y)$, the cost of the only simple path from vertex $x$ to $y$ in the key tree is equal to the <span class="tex-font-style-bf">minimum cost</span> of a simple circuit that goes through vertices $x$ and $y$ in the graph. </li></ul> </li><li> Note that the graph is allowed to have multi-edges, but is not allowed to have self-loops. </li></ul><p>Print the answer modulo $998\,244\,353$.</p><p>Two graphs are considered distinct if and only if there exists a triple $(a, b, c)$ such that there exists an edge that connects vertices $a$ and $b$ with weight $c$ in one graph, but not in the other.</p></div><div class="input-specification"><p>The first line contains a single integer $N$ ($2 \le N \le 10^5$) — the number of vertices in the key tree.</p><p>The $i$-th of the next $N-1$ lines contains two integers $U_i$ and $V_i$ ($1 \le U_i, V_i \le N$) — an edge connecting vertices $U_i$ and $V_i$. The graph in the input is a tree.</p></div><div class="output-specification"><p>An integer representing the number of distinct undirected weighted graphs that satisfy the conditions of the problem modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a single integer $N$ ($2 \le N \le 10^5$) — the number of vertices in the key tree.</p><p>The $i$-th of the next $N-1$ lines contains two integers $U_i$ and $V_i$ ($1 \le U_i, V_i \le N$) — an edge connecting vertices $U_i$ and $V_i$. The graph in the input is a tree.</p>

## Output

<p>An integer representing the number of distinct undirected weighted graphs that satisfy the conditions of the problem modulo $998\,244\,353$.</p>





```input1
4
3 2
1 3
4 3
```




```output1
540
```



## Note

<p>The following is an example of a graph that satisfies.</p><p><img class="tex-graphics" src="file://rXIK328d.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The following is an assignment of edge weights in the key tree that corresponds to the graph above.</p><p><img class="tex-graphics" src="file://oWnxzIoc.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>As an example, consider a pair of vertex indices $(1, 4)$. </p><ul> <li> The circuit in the graph for this pair of vertices is $3 \xrightarrow{2} 2 \xrightarrow{4} 4 \xrightarrow{6} 2 \xrightarrow{1} 1 \xrightarrow{5} 3$ with a cost of $6$. </li><li> The path in the key tree for this pair of vertices is $1 \xrightarrow{5} 3 \xrightarrow{6} 4$ with a cost of $6$. </li></ul>
