## Description

<div><p>You are given $n$ integers $a_1, a_2, \ldots, a_n$. For any real number $t$, consider the complete weighted graph on $n$ vertices $K_n(t)$ with weight of the edge between vertices $i$ and $j$ equal to $w_{ij}(t) = a_i \cdot a_j + t \cdot (a_i + a_j)$. </p><p>Let $f(t)$ be the cost of the <a href="https://en.wikipedia.org/wiki/Minimum_spanning_tree">minimum spanning tree</a> of $K_n(t)$. Determine whether $f(t)$ is bounded above and, if so, output the maximum value it attains.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $T$ ($1 \leq T \leq 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2 \cdot 10^5$) — the number of vertices of the graph.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^6 \leq a_i \leq 10^6$).</p><p>The sum of $n$ for all test cases is at most $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line with the maximum value of $f(t)$ (it can be shown that it is an integer), or <span class="tex-font-style-tt">INF</span> if $f(t)$ is not bounded above. </p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $T$ ($1 \leq T \leq 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2 \cdot 10^5$) — the number of vertices of the graph.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^6 \leq a_i \leq 10^6$).</p><p>The sum of $n$ for all test cases is at most $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single line with the maximum value of $f(t)$ (it can be shown that it is an integer), or <span class="tex-font-style-tt">INF</span> if $f(t)$ is not bounded above. </p>





```input1|2,3,6,7,10,11
5
2
1 0
2
-1 1
3
1 -1 -2
3
3 -1 -2
4
1 2 3 -4
```




```output1
INF
-1
INF
-6
-18
```


