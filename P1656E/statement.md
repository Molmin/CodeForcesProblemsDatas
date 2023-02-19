## Description

<div><p>You are given an undirected unrooted tree, i.e. a connected undirected graph without cycles.</p><p>You must assign a <span class="tex-font-style-bf">nonzero</span> integer weight to each vertex so that the following is satisfied: if any vertex of the tree is removed, then each of the remaining connected components has the same sum of weights in its vertices.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($3 \leq n \leq 10^5$) — the number of vertices of the tree.</p><p>The next $n-1$ lines of each case contain each two integers $u, v$ ($1 \leq u,v \leq n$) denoting that there is an edge between vertices $u$ and $v$. It is guaranteed that the given edges form a tree.</p><p>The sum of $n$ for all test cases is at most $10^5$.</p></div><div class="output-specification"><p>For each test case, you must output one line with $n$ space separated integers $a_1, a_2, \ldots, a_n$, where $a_i$ is the weight assigned to vertex $i$. <span class="tex-font-style-bf">The weights must satisfy $-10^5 \leq a_i \leq 10^5$ and $a_i \neq 0$.</span></p><p>It can be shown that there always exists a solution satisfying these constraints. If there are multiple possible solutions, output any of them.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($3 \leq n \leq 10^5$) — the number of vertices of the tree.</p><p>The next $n-1$ lines of each case contain each two integers $u, v$ ($1 \leq u,v \leq n$) denoting that there is an edge between vertices $u$ and $v$. It is guaranteed that the given edges form a tree.</p><p>The sum of $n$ for all test cases is at most $10^5$.</p>

## Output

<p>For each test case, you must output one line with $n$ space separated integers $a_1, a_2, \ldots, a_n$, where $a_i$ is the weight assigned to vertex $i$. <span class="tex-font-style-bf">The weights must satisfy $-10^5 \leq a_i \leq 10^5$ and $a_i \neq 0$.</span></p><p>It can be shown that there always exists a solution satisfying these constraints. If there are multiple possible solutions, output any of them.</p>





```input1
2
5
1 2
1 3
3 4
3 5
3
1 2
1 3
```




```output1
-3 5 1 2 2
1 1 1
```



## Note

<p>In the first case, when removing vertex $1$ all remaining connected components have sum $5$ and when removing vertex $3$ all remaining connected components have sum $2$. When removing other vertices, there is only one remaining connected component so all remaining connected components have the same sum.</p>
