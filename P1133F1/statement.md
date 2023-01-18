## Description

<div><p>You are given an undirected unweighted connected graph consisting of $n$ vertices and $m$ edges. It is guaranteed that there are no self-loops or multiple edges in the given graph.</p><p>Your task is to find <span class="tex-font-style-bf">any</span> spanning tree of this graph such that the maximum degree over all vertices is maximum possible. Recall that the degree of a vertex is the number of edges incident to it.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $n - 1 \le m \le min(2 \cdot 10^5, \frac{n(n-1)}{2})$) — the number of vertices and edges, respectively.</p><p>The following $m$ lines denote edges: edge $i$ is represented by a pair of integers $v_i$, $u_i$ ($1 \le v_i, u_i \le n$, $u_i \ne v_i$), which are the indices of vertices connected by the edge. There are no loops or multiple edges in the given graph, i. e. for each pair ($v_i, u_i$) there are no other pairs ($v_i, u_i$) or ($u_i, v_i$) in the list of edges, and for each pair $(v_i, u_i)$ the condition $v_i \ne u_i$ is satisfied.</p></div><div class="output-specification"><p>Print $n-1$ lines describing the edges of a spanning tree such that the maximum degree over all vertices is maximum possible. Make sure that the edges of the printed spanning tree form some subset of the input edges (order doesn't matter and edge $(v, u)$ is considered the same as the edge $(u, v)$).</p><p>If there are multiple possible answers, print any of them.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $n - 1 \le m \le min(2 \cdot 10^5, \frac{n(n-1)}{2})$) — the number of vertices and edges, respectively.</p><p>The following $m$ lines denote edges: edge $i$ is represented by a pair of integers $v_i$, $u_i$ ($1 \le v_i, u_i \le n$, $u_i \ne v_i$), which are the indices of vertices connected by the edge. There are no loops or multiple edges in the given graph, i. e. for each pair ($v_i, u_i$) there are no other pairs ($v_i, u_i$) or ($u_i, v_i$) in the list of edges, and for each pair $(v_i, u_i)$ the condition $v_i \ne u_i$ is satisfied.</p>

## Output

<p>Print $n-1$ lines describing the edges of a spanning tree such that the maximum degree over all vertices is maximum possible. Make sure that the edges of the printed spanning tree form some subset of the input edges (order doesn't matter and edge $(v, u)$ is considered the same as the edge $(u, v)$).</p><p>If there are multiple possible answers, print any of them.</p>





```input1
5 5
1 2
2 3
3 5
4 3
1 5
```




```input2
4 6
1 2
1 3
1 4
2 3
2 4
3 4
```




```input3
8 9
1 2
2 3
2 5
1 6
3 4
6 5
4 5
2 7
5 8
```




```output1
3 5
2 1
3 2
3 4
```




```output2
4 1
1 2
1 3
```




```output3
3 2
2 5
8 5
6 1
2 7
1 2
3 4
```



## Note

<p>Picture corresponding to the first example: <img class="tex-graphics" src="file://WuYXqIUd.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In this example the number of edges of spanning tree incident to the vertex $3$ is $3$. It is the maximum degree over all vertices of the spanning tree. It is easy to see that we cannot obtain a better answer.</p><p>Picture corresponding to the second example: <img class="tex-graphics" src="file://Yv8nkLF4.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In this example the number of edges of spanning tree incident to the vertex $1$ is $3$. It is the maximum degree over all vertices of the spanning tree. It is easy to see that we cannot obtain a better answer.</p><p>Picture corresponding to the third example: <img class="tex-graphics" src="file://PIoM2vhs.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In this example the number of edges of spanning tree incident to the vertex $2$ is $4$. It is the maximum degree over all vertices of the spanning tree. It is easy to see that we cannot obtain a better answer. But because this example is symmetric, we can choose almost the same spanning tree but with vertex $5$ instead of $2$.</p>
