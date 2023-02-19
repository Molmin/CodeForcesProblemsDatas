## Description

<div><p>CQXYM wants to create a connected undirected graph with $n$ nodes and $m$ edges, and the diameter of the graph must be strictly less than $k-1$. Also, CQXYM doesn't want a graph that contains self-loops or multiple edges (i.e. each edge connects two different vertices and between each pair of vertices there is at most one edge).</p><p>The diameter of a graph is the maximum distance between any two nodes.</p><p>The distance between two nodes is the minimum number of the edges on the path which endpoints are the two nodes.</p><p>CQXYM wonders whether it is possible to create such a graph.</p></div><div class="input-specification"><p>The input consists of multiple test cases. </p><p>The first line contains an integer $t (1 \leq t \leq 10^5)$ — the number of test cases. The description of the test cases follows.</p><p>Only one line of each test case contains three integers $n(1 \leq n \leq 10^9)$, $m$, $k$ $(0 \leq m,k \leq 10^9)$.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to create the graph, or print <span class="tex-font-style-tt">NO</span> if it is impossible. You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The input consists of multiple test cases. </p><p>The first line contains an integer $t (1 \leq t \leq 10^5)$ — the number of test cases. The description of the test cases follows.</p><p>Only one line of each test case contains three integers $n(1 \leq n \leq 10^9)$, $m$, $k$ $(0 \leq m,k \leq 10^9)$.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to create the graph, or print <span class="tex-font-style-tt">NO</span> if it is impossible. You can print each letter in any case (upper or lower).</p>





```input1
5
1 0 3
4 5 3
4 6 3
5 4 1
2 1 1
```




```output1
YES
NO
YES
NO
NO
```



## Note

<p>In the first test case, the graph's diameter equal to 0.</p><p>In the second test case, the graph's diameter can only be 2.</p><p>In the third test case, the graph's diameter can only be 1.</p>
