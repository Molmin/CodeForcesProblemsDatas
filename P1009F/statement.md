## Description

<div><p>You are given a rooted undirected tree consisting of $n$ vertices. Vertex $1$ is the root.</p><p>Let's denote a <span class="tex-font-style-it">depth array</span> of vertex $x$ as an infinite sequence $[d_{x, 0}, d_{x, 1}, d_{x, 2}, \dots]$, where $d_{x, i}$ is the number of vertices $y$ such that both conditions hold:</p><ul> <li> $x$ is an ancestor of $y$; </li><li> the simple path from $x$ to $y$ traverses exactly $i$ edges. </li></ul><p>The <span class="tex-font-style-it">dominant index</span> of a <span class="tex-font-style-it">depth array</span> of vertex $x$ (or, shortly, the <span class="tex-font-style-it">dominant index</span> of vertex $x$) is an index $j$ such that:</p><ul> <li> for every $k &lt; j$, $d_{x, k} &lt; d_{x, j}$; </li><li> for every $k &gt; j$, $d_{x, k} \le d_{x, j}$. </li></ul><p>For every vertex in the tree calculate its <span class="tex-font-style-it">dominant index</span>.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 10^6$) — the number of vertices in a tree.</p><p>Then $n - 1$ lines follow, each containing two integers $x$ and $y$ ($1 \le x, y \le n$, $x \ne y$). This line denotes an edge of the tree.</p><p>It is guaranteed that these edges form a tree.</p></div><div class="output-specification"><p>Output $n$ numbers. $i$-th number should be equal to the <span class="tex-font-style-it">dominant index</span> of vertex $i$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 10^6$) — the number of vertices in a tree.</p><p>Then $n - 1$ lines follow, each containing two integers $x$ and $y$ ($1 \le x, y \le n$, $x \ne y$). This line denotes an edge of the tree.</p><p>It is guaranteed that these edges form a tree.</p>

## Output

<p>Output $n$ numbers. $i$-th number should be equal to the <span class="tex-font-style-it">dominant index</span> of vertex $i$.</p>





```input1
4
1 2
2 3
3 4

```




```input2
4
1 2
1 3
1 4

```




```input3
4
1 2
2 3
2 4

```




```output1
0
0
0
0

```




```output2
1
0
0
0

```




```output3
2
1
0
0

```


