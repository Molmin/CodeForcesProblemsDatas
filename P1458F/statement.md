## Description

<div><p>You are given a tree with $n$ vertices numbered $1, \ldots, n$. A tree is a connected simple graph without cycles.</p><p>Let $\mathrm{dist}(u, v)$ be the number of edges in the unique simple path connecting vertices $u$ and $v$.</p><p>Let $\mathrm{diam}(l, r) = \max \mathrm{dist}(u, v)$ over all pairs $u, v$ such that $l \leq u, v \leq r$.</p><p>Compute $\sum_{1 \leq l \leq r \leq n} \mathrm{diam}(l, r)$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the number of vertices in the tree.</p><p>The next $n - 1$ lines describe the tree edges. Each of these lines contains two integers $u, v$ ($1 \leq u, v \leq n$)&nbsp;— endpoint indices of the respective tree edge. It is guaranteed that the edge list indeed describes a tree.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— $\sum_{1 \leq l \leq r \leq n} \mathrm{diam}(l, r)$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the number of vertices in the tree.</p><p>The next $n - 1$ lines describe the tree edges. Each of these lines contains two integers $u, v$ ($1 \leq u, v \leq n$)&nbsp;— endpoint indices of the respective tree edge. It is guaranteed that the edge list indeed describes a tree.</p>

## Output

<p>Print a single integer&nbsp;— $\sum_{1 \leq l \leq r \leq n} \mathrm{diam}(l, r)$.</p>





```input1
4
1 2
2 4
3 2
```




```input2
10
1 8
2 9
5 6
4 8
4 2
7 9
3 6
10 4
3 9
```




```output1
10
```




```output2
224
```


