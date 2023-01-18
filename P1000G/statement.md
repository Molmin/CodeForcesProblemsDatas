## Description

<div><p>You are given a weighted tree (undirected connected graph with no cycles, loops or multiple edges) with $n$ vertices. The edge $\{u_j, v_j\}$ has weight $w_j$. Also each vertex $i$ has its own value $a_i$ assigned to it.</p><p>Let's call a path starting in vertex $u$ and ending in vertex $v$, where each edge can appear no more than twice (regardless of direction), a <span class="tex-font-style-it">2-path</span>. Vertices can appear in the 2-path multiple times (even start and end vertices).</p><p>For some 2-path $p$ profit $\text{Pr}(p) = \sum\limits_{v \in \text{distinct vertices in } p}{a_v} - \sum\limits_{e \in \text{distinct edges in } p}{k_e \cdot w_e}$, where $k_e$ is the number of times edge $e$ appears in $p$. That is, vertices are counted once, but edges are counted the number of times they appear in $p$.</p><p>You are about to answer $m$ queries. Each query is a pair of vertices $(qu, qv)$. For each query find 2-path $p$ from $qu$ to $qv$ with maximal profit $\text{Pr}(p)$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($2 \le n \le 3 \cdot 10^5$, $1 \le q \le 4 \cdot 10^5$) — the number of vertices in the tree and the number of queries.</p><p>The second line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 10^9)$ — the values of the vertices.</p><p>Next $n - 1$ lines contain descriptions of edges: each line contains three space separated integers $u_i$, $v_i$ and $w_i$ ($1 \le u_i, v_i \le n$, $u_i \neq v_i$, $1 \le w_i \le 10^9$) — there is edge $\{u_i, v_i\}$ with weight $w_i$ in the tree.</p><p>Next $q$ lines contain queries (one per line). Each query contains two integers $qu_i$ and $qv_i$ $(1 \le qu_i, qv_i \le n)$ — endpoints of the 2-path you need to find.</p></div><div class="output-specification"><p>For each query print one integer per line — maximal profit $\text{Pr}(p)$ of the some 2-path $p$ with the corresponding endpoints.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($2 \le n \le 3 \cdot 10^5$, $1 \le q \le 4 \cdot 10^5$) — the number of vertices in the tree and the number of queries.</p><p>The second line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 10^9)$ — the values of the vertices.</p><p>Next $n - 1$ lines contain descriptions of edges: each line contains three space separated integers $u_i$, $v_i$ and $w_i$ ($1 \le u_i, v_i \le n$, $u_i \neq v_i$, $1 \le w_i \le 10^9$) — there is edge $\{u_i, v_i\}$ with weight $w_i$ in the tree.</p><p>Next $q$ lines contain queries (one per line). Each query contains two integers $qu_i$ and $qv_i$ $(1 \le qu_i, qv_i \le n)$ — endpoints of the 2-path you need to find.</p>

## Output

<p>For each query print one integer per line — maximal profit $\text{Pr}(p)$ of the some 2-path $p$ with the corresponding endpoints.</p>





```input1
7 6
6 5 5 3 2 1 2
1 2 2
2 3 2
2 4 1
4 5 1
6 4 2
7 3 25
1 1
4 4
5 6
6 4
3 4
3 7

```




```output1
9
9
9
8
12
-14

```



## Note

<p>Explanation of queries: </p><ol> <li> $(1, 1)$ — one of the optimal 2-paths is the following: $1 \rightarrow 2 \rightarrow 4 \rightarrow 5 \rightarrow 4 \rightarrow 2 \rightarrow 3 \rightarrow 2 \rightarrow 1$. $\text{Pr}(p) = (a_1 + a_2 + a_3 + a_4 + a_5) - (2 \cdot w(1,2) + 2 \cdot w(2,3) + 2 \cdot w(2,4) + 2 \cdot w(4,5)) = 21 - 2 \cdot 12 = 9$. </li><li> $(4, 4)$: $4 \rightarrow 2 \rightarrow 1 \rightarrow 2 \rightarrow 3 \rightarrow 2 \rightarrow 4$. $\text{Pr}(p) = (a_1 + a_2 + a_3 + a_4) - 2 \cdot (w(1,2) + w(2,3) + w(2,4)) = 19 - 2 \cdot 10 = 9$. </li><li> $(5, 6)$: $5 \rightarrow 4 \rightarrow 2 \rightarrow 3 \rightarrow 2 \rightarrow 1 \rightarrow 2 \rightarrow 4 \rightarrow 6$. </li><li> $(6, 4)$: $6 \rightarrow 4 \rightarrow 2 \rightarrow 1 \rightarrow 2 \rightarrow 3 \rightarrow 2 \rightarrow 4$. </li><li> $(3, 4)$: $3 \rightarrow 2 \rightarrow 1 \rightarrow 2 \rightarrow 4$. </li><li> $(3, 7)$: $3 \rightarrow 2 \rightarrow 1 \rightarrow 2 \rightarrow 4 \rightarrow 5 \rightarrow 4 \rightarrow 2 \rightarrow 3 \rightarrow 7$. </li></ol>
