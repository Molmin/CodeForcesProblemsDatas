## Description

<div><p>Given an undirected graph $G$, we say that a <span class="tex-font-style-it">neighbour ordering</span> is an ordered list of all the neighbours of a vertex for each of the vertices of $G$. Consider a given neighbour ordering of $G$ and three vertices $u$, $v$ and $w$, such that $v$ is a neighbor of $u$ and $w$. We write $u &lt;_{v} w$ if $u$ comes after $w$ in $v$'s neighbor list.</p><p>A neighbour ordering is said to be <span class="tex-font-style-it">good</span> if, for each simple cycle $v_1, v_2, \ldots, v_c$ of the graph, one of the following is satisfied:</p><ul> <li> $v_1 &lt;_{v_2} v_3, v_2 &lt;_{v_3} v_4, \ldots, v_{c-2} &lt;_{v_{c-1}} v_c, v_{c-1} &lt;_{v_c} v_1, v_c &lt;_{v_1} v_2$.</li><li> $v_1 &gt;_{v_2} v_3, v_2 &gt;_{v_3} v_4, \ldots, v_{c-2} &gt;_{v_{c-1}} v_c, v_{c-1} &gt;_{v_c} v_1, v_c &gt;_{v_1} v_2$. </li></ul><p>Given a graph $G$, determine whether there exists a good neighbour ordering for it and construct one if it does.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq 3 \cdot 10^5$, $1 \leq m \leq 3 \cdot 10^5$), the number of vertices and the number of edges of the graph.</p><p>The next $m$ lines each contain two integers $u, v$ ($0 \leq u, v &lt; n$), denoting that there is an edge connecting vertices $u$ and $v$. It is guaranteed that the graph is connected and there are no loops or multiple edges between the same vertices.</p><p>The sum of $n$ and the sum of $m$ for all test cases are at most $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output one line with <span class="tex-font-style-tt">YES</span> if there is a good neighbour ordering, otherwise output one line with <span class="tex-font-style-tt">NO</span>. You can print each letter in any case (upper or lower).</p><p>If the answer is <span class="tex-font-style-tt">YES</span>, additionally output $n$ lines describing a good neighbour ordering. In the $i$-th line, output the neighbours of vertex $i$ in order. </p><p>If there are multiple good neigbour orderings, print any.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq 3 \cdot 10^5$, $1 \leq m \leq 3 \cdot 10^5$), the number of vertices and the number of edges of the graph.</p><p>The next $m$ lines each contain two integers $u, v$ ($0 \leq u, v &lt; n$), denoting that there is an edge connecting vertices $u$ and $v$. It is guaranteed that the graph is connected and there are no loops or multiple edges between the same vertices.</p><p>The sum of $n$ and the sum of $m$ for all test cases are at most $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output one line with <span class="tex-font-style-tt">YES</span> if there is a good neighbour ordering, otherwise output one line with <span class="tex-font-style-tt">NO</span>. You can print each letter in any case (upper or lower).</p><p>If the answer is <span class="tex-font-style-tt">YES</span>, additionally output $n$ lines describing a good neighbour ordering. In the $i$-th line, output the neighbours of vertex $i$ in order. </p><p>If there are multiple good neigbour orderings, print any.</p>





```input1
3
5 6
0 1
0 2
1 2
2 3
3 4
4 1
2 1
0 1
6 10
0 1
2 0
0 3
0 4
1 2
1 4
2 3
2 5
3 5
4 5
```




```output1
YES
1 2 
4 2 0 
0 1 3 
2 4 
3 1 
YES
1 
0 
NO
```


