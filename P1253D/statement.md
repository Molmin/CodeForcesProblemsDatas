## Description

<div><p>You're given an undirected graph with $n$ nodes and $m$ edges. Nodes are numbered from $1$ to $n$.</p><p>The graph is considered <span class="tex-font-style-it">harmonious</span> if and only if the following property holds:</p><ul> <li> For every triple of integers $(l, m, r)$ such that $1 \le l &lt; m &lt; r \le n$, if there exists a <span class="tex-font-style-bf">path</span> going from node $l$ to node $r$, then there exists a <span class="tex-font-style-bf">path</span> going from node $l$ to node $m$. </li></ul><p>In other words, in a harmonious graph, if from a node $l$ we can reach a node $r$ through edges ($l &lt; r$), then we should able to reach nodes $(l+1), (l+2), \ldots, (r-1)$ too.</p><p>What is the minimum number of edges we need to add to make the graph harmonious? </p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($3 \le n \le 200\ 000$ and $1 \le m \le 200\ 000$).</p><p>The $i$-th of the next $m$ lines contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$, $u_i \neq v_i$), that mean that there's an edge between nodes $u$ and $v$.</p><p>It is guaranteed that the given graph is simple (there is no self-loop, and there is at most one edge between every pair of nodes).</p></div><div class="output-specification"><p>Print the minimum number of edges we have to add to the graph to make it harmonious.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($3 \le n \le 200\ 000$ and $1 \le m \le 200\ 000$).</p><p>The $i$-th of the next $m$ lines contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$, $u_i \neq v_i$), that mean that there's an edge between nodes $u$ and $v$.</p><p>It is guaranteed that the given graph is simple (there is no self-loop, and there is at most one edge between every pair of nodes).</p>

## Output

<p>Print the minimum number of edges we have to add to the graph to make it harmonious.</p>





```input1
14 8
1 2
2 7
3 4
6 3
5 7
3 8
6 8
11 12
```




```input2
200000 3
7 9
9 8
4 5
```




```output1
1
```




```output2
0
```



## Note

<p>In the first example, the given graph is not harmonious (for instance, $1 &lt; 6 &lt; 7$, node $1$ can reach node $7$ through the path $1 \rightarrow 2 \rightarrow 7$, but node $1$ can't reach node $6$). However adding the edge $(2, 4)$ is sufficient to make it harmonious.</p><p>In the second example, the given graph is already harmonious.</p>
