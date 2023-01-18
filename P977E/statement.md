## Description

<div><p>You are given an undirected graph consisting of $n$ vertices and $m$ edges. Your task is to find the number of connected components which are cycles.</p><p>Here are some definitions of graph theory.</p><p>An undirected graph consists of two sets: set of nodes (called vertices) and set of edges. Each edge connects a pair of vertices. All edges are bidirectional (i.e. if a vertex $a$ is connected with a vertex $b$, a vertex $b$ is also connected with a vertex $a$). An edge can't connect vertex with itself, there is at most one edge between a pair of vertices.</p><p>Two vertices $u$ and $v$ belong to the same connected component if and only if there is at least one path along edges connecting $u$ and $v$.</p><p>A connected component is a cycle if and only if its vertices can be reordered in such a way that:</p><ul> <li> the first vertex is connected with the second vertex by an edge, </li><li> the second vertex is connected with the third vertex by an edge, </li><li> ... </li><li> the last vertex is connected with the first vertex by an edge, </li><li> all the described edges of a cycle are distinct. </li></ul><p>A cycle doesn't contain any other edges except described above. By definition any cycle contains three or more vertices.</p><center> <img class="tex-graphics" src="file://4Zy0yJhC.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">There are $6$ connected components, $2$ of them are cycles: $[7, 10, 16]$ and $[5, 11, 9, 15]$.</span> </center></div><div class="input-specification"><p>The first line contains two integer numbers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$, $0 \le m \le 2 \cdot 10^5$) — number of vertices and edges.</p><p>The following $m$ lines contains edges: edge $i$ is given as a pair of vertices $v_i$, $u_i$ ($1 \le v_i, u_i \le n$, $u_i \ne v_i$). There is no multiple edges in the given graph, i.e. for each pair ($v_i, u_i$) there no other pairs ($v_i, u_i$) and ($u_i, v_i$) in the list of edges.</p></div><div class="output-specification"><p>Print one integer — the number of connected components which are also cycles.</p></div>

## Input

<p>The first line contains two integer numbers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$, $0 \le m \le 2 \cdot 10^5$) — number of vertices and edges.</p><p>The following $m$ lines contains edges: edge $i$ is given as a pair of vertices $v_i$, $u_i$ ($1 \le v_i, u_i \le n$, $u_i \ne v_i$). There is no multiple edges in the given graph, i.e. for each pair ($v_i, u_i$) there no other pairs ($v_i, u_i$) and ($u_i, v_i$) in the list of edges.</p>

## Output

<p>Print one integer — the number of connected components which are also cycles.</p>





```input1
5 4
1 2
3 4
5 4
3 5

```




```input2
17 15
1 8
1 12
5 11
11 9
9 15
15 5
4 13
3 13
4 3
10 16
7 10
16 7
14 3
14 4
17 6

```




```output1
1

```




```output2
2

```



## Note

<p>In the first example only component $[3, 4, 5]$ is also a cycle.</p><p>The illustration above corresponds to the second example.</p>
