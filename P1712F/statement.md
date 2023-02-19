## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">&nbsp;— What is my mission?</span></div></div> <div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">&nbsp;— To count graph diameters.</span></div><div class="epigraph-source">You and Your Submission</div></div><p>A tree is a connected undirected graph without cycles. A weighted tree has a weight assigned to each edge. The degree of a vertex is the number of edges connected to this vertex.</p><p>You are given a weighted tree with $n$ vertices, each edge has a weight of $1$. Let $L$ be the set of vertices with degree equal to $1$. </p><p>You have to answer $q$ <span class="tex-font-style-bf">independent</span> queries. In the $i$-th query:</p><ol> <li> You are given a positive integer $x_i$. </li><li> For all $u,v \in L$ such that $u &lt; v$, add edge $(u, v)$ with weight $x_i$ to the graph (initially the given tree). </li><li> Find the diameter of the resulting graph. </li></ol><p>The diameter of a graph is equal to $\max\limits_{1 \le u &lt; v \le n}{\operatorname{d}(u, v)}$, where $\operatorname{d}(u, v)$ is the length of the shortest path between vertex $u$ and vertex $v$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($3 \le n \le 10^6$).</p><p>The second line contains $n - 1$ integers $p_2,p_3,\ldots,p_n$ ($1 \le p_i &lt; i$) indicating that there is an edge between vertices $i$ and $p_i$. It is guaranteed that the given edges form a tree.</p><p>The third line contains a single integer $q$ ($1 \le q \le 10$).</p><p>The fourth line contains $q$ integers $x_1,x_2,\ldots,x_q$ ($1 \le x_i \le n$). All $x_i$ are <span class="tex-font-style-bf">distinct</span>.</p></div><div class="output-specification"><p>Print $q$ integers in a single line — the answers to the queries.</p></div>

## Input

<p>The first line contains a single integer $n$ ($3 \le n \le 10^6$).</p><p>The second line contains $n - 1$ integers $p_2,p_3,\ldots,p_n$ ($1 \le p_i &lt; i$) indicating that there is an edge between vertices $i$ and $p_i$. It is guaranteed that the given edges form a tree.</p><p>The third line contains a single integer $q$ ($1 \le q \le 10$).</p><p>The fourth line contains $q$ integers $x_1,x_2,\ldots,x_q$ ($1 \le x_i \le n$). All $x_i$ are <span class="tex-font-style-bf">distinct</span>.</p>

## Output

<p>Print $q$ integers in a single line — the answers to the queries.</p>





```input1
4
1 2 2
4
1 2 3 4
```




```input2
7
1 2 3 4 2 1
7
2 1 3 7 5 6 4
```




```input3
3
1 2
1
1
```




```output1
1 2 2 2
```




```output2
3 3 4 5 5 5 4
```




```output3
1
```



## Note

<p>The graph in the first test after adding the edges: </p><center> <img class="tex-graphics" src="file://YbXzGx5h.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
