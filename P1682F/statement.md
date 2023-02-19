## Description

<div><p>You are given two integer arrays $a$ and $b$ ($b_i \neq 0$ and $|b_i| \leq 10^9$). Array $a$ is sorted in <span class="tex-font-style-bf">non-decreasing</span> order.</p><p>The cost of a subarray $a[l:r]$ is defined as follows:</p><ul><li><p>If $ \sum\limits_{j = l}^{r} b_j \neq 0$, then the cost is not defined.</p></li><li><p>Otherwise:</p><ul><li> Construct a bipartite flow graph with $r-l+1$ vertices, labeled from $l$ to $r$, with all vertices having $b_i \lt 0$ on the left and those with $b_i \gt 0$ on right. For each $i, j$ such that $l \le i, j \le r$, $b_i&lt;0$ and $b_j&gt;0$, draw an edge from $i$ to $j$ with infinite capacity and cost of unit flow as $|a_i-a_j|$.</li><li> Add two more vertices: source $S$ and sink $T$.</li><li> For each $i$ such that $l \le i \le r$ and $b_i&lt;0$, add an edge from $S$ to $i$ with cost $0$ and capacity $|b_i|$.</li><li> For each $i$ such that $l \le i \le r$ and $b_i&gt;0$, add an edge from $i$ to $T$ with cost $0$ and capacity $|b_i|$.</li><li> The cost of the subarray is then defined as the minimum cost of maximum flow from $S$ to $T$.</li></ul></li></ul><p>You are given $q$ queries in the form of two integers $l$ and $r$. You have to compute the cost of subarray $a[l:r]$ for each query, modulo $10^9 + 7$.</p><p>If you don't know what the minimum cost of maximum flow means, read <a href="https://en.wikipedia.org/wiki/Minimum-cost_flow_problem">here</a>.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $q$ $(2 \leq n \leq 2\cdot 10^5, 1 \leq q \leq 2\cdot10^5)$ &nbsp;— length of arrays $a$, $b$ and the number of queries.</p><p>The next line contains $n$ integers $a_1,a_2 \ldots a_n$ ($0 \leq a_1 \le a_2 \ldots \le a_n \leq 10^9)$ &nbsp;— the array $a$. It is guaranteed that $a$ is sorted in <span class="tex-font-style-bf">non-decreasing</span> order.</p><p>The next line contains $n$ integers $b_1,b_2 \ldots b_n$ $(-10^9\leq b_i \leq 10^9, b_i \neq 0)$ &nbsp;— the array $b$.</p><p>The $i$-th of the next $q$ lines contains two integers $l_i,r_i$ $(1\leq l_i \leq r_i \leq n)$. It is guaranteed that $ \sum\limits_{j = l_i}^{r_i} b_j = 0$.</p></div><div class="output-specification"><p>For each query $l_i$, $r_i$ &nbsp;— print the cost of subarray $a[l_i:r_i]$ modulo $10^9 + 7$.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $q$ $(2 \leq n \leq 2\cdot 10^5, 1 \leq q \leq 2\cdot10^5)$ &nbsp;— length of arrays $a$, $b$ and the number of queries.</p><p>The next line contains $n$ integers $a_1,a_2 \ldots a_n$ ($0 \leq a_1 \le a_2 \ldots \le a_n \leq 10^9)$ &nbsp;— the array $a$. It is guaranteed that $a$ is sorted in <span class="tex-font-style-bf">non-decreasing</span> order.</p><p>The next line contains $n$ integers $b_1,b_2 \ldots b_n$ $(-10^9\leq b_i \leq 10^9, b_i \neq 0)$ &nbsp;— the array $b$.</p><p>The $i$-th of the next $q$ lines contains two integers $l_i,r_i$ $(1\leq l_i \leq r_i \leq n)$. It is guaranteed that $ \sum\limits_{j = l_i}^{r_i} b_j = 0$.</p>

## Output

<p>For each query $l_i$, $r_i$ &nbsp;— print the cost of subarray $a[l_i:r_i]$ modulo $10^9 + 7$.</p>





```input1
8 4
1 2 4 5 9 10 10 13
6 -1 1 -3 2 1 -1 1
2 3
6 7
3 5
2 6
```




```output1
2
0
9
15
```



## Note

<p>In the <span class="tex-font-style-bf">first query</span>, the maximum possible flow is $1$ i.e one unit from source to $2$, then one unit from $2$ to $3$, then one unit from $3$ to sink. The cost of the flow is $0 \cdot 1 + |2 - 4| \cdot 1 + 0 \cdot 1 = 2$.</p><p>In the <span class="tex-font-style-bf">second query</span>, the maximum possible flow is again $1$ i.e from source to $7$, $7$ to $6$, and $6$ to sink with a cost of $0 \cdot |10 - 10| \cdot 1 + 0 \cdot 1 = 0$. </p><p>In the <span class="tex-font-style-bf">third query</span>, the flow network is shown on the left with capacity written over the edge and the cost written in bracket. The image on the right shows the flow through each edge in an optimal configuration. </p><center> <img class="tex-graphics" src="file://rD2Lv7Rx.png" style="max-width: 100.0%;max-height: 100.0%;" width="1512px"> </center> Maximum flow is $3$ with a cost of $0 \cdot 3 + 1 \cdot 1 + 4 \cdot 2 + 0 \cdot 1 + 0 \cdot 2 = 9$.<p>In the <span class="tex-font-style-bf">fourth query</span>, the flow network looks as – </p><center> <img class="tex-graphics" height="265px" src="file://jDeqq6QL.png" style="max-width: 100.0%;max-height: 100.0%;" width="491px"> </center><p>The minimum cost maximum flow is achieved in the configuration – </p><center> <img class="tex-graphics" height="265px" src="file://R03hXS2I.png" style="max-width: 100.0%;max-height: 100.0%;" width="491px"> </center><p>The maximum flow in the above network is 4 and the minimum cost of such flow is 15.</p>
