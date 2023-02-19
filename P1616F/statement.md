## Description

<div><p>You are given a simple undirected graph with $n$ vertices and $m$ edges. Edge $i$ is colored in the color $c_i$, which is either $1$, $2$, or $3$, or left uncolored (in this case, $c_i = -1$).</p><p>You need to color all of the uncolored edges in such a way that for any three pairwise adjacent vertices $1 \leq a &lt; b &lt; c \leq n$, the colors of the edges $a \leftrightarrow b$, $b \leftrightarrow c$, and $a \leftrightarrow c$ are either pairwise different, or all equal. In case no such coloring exists, you need to determine that.</p></div><div class="input-specification"><p>The first line of input contains one integer $t$ ($1 \leq t \leq 10$): the number of test cases.</p><p>The following lines contain the description of the test cases.</p><p>In the first line you are given two integers $n$ and $m$ ($3 \leq n \leq 64$, $0 \leq m \leq \min(256, \frac{n(n-1)}{2})$): the number of vertices and edges in the graph.</p><p>Each of the next $m$ lines contains three integers $a_i$, $b_i$, and $c_i$ ($1 \leq a_i, b_i \leq n$, $a_i \ne b_i$, $c_i$ is either $-1$, $1$, $2$, or $3$), denoting an edge between $a_i$ and $b_i$ with color $c_i$. It is guaranteed that no two edges share the same endpoints.</p></div><div class="output-specification"><p>For each test case, print $m$ integers $d_1, d_2, \ldots, d_m$, where $d_i$ is the color of the $i$-th edge in your final coloring. If there is no valid way to finish the coloring, print $-1$.</p></div>

## Input

<p>The first line of input contains one integer $t$ ($1 \leq t \leq 10$): the number of test cases.</p><p>The following lines contain the description of the test cases.</p><p>In the first line you are given two integers $n$ and $m$ ($3 \leq n \leq 64$, $0 \leq m \leq \min(256, \frac{n(n-1)}{2})$): the number of vertices and edges in the graph.</p><p>Each of the next $m$ lines contains three integers $a_i$, $b_i$, and $c_i$ ($1 \leq a_i, b_i \leq n$, $a_i \ne b_i$, $c_i$ is either $-1$, $1$, $2$, or $3$), denoting an edge between $a_i$ and $b_i$ with color $c_i$. It is guaranteed that no two edges share the same endpoints.</p>

## Output

<p>For each test case, print $m$ integers $d_1, d_2, \ldots, d_m$, where $d_i$ is the color of the $i$-th edge in your final coloring. If there is no valid way to finish the coloring, print $-1$.</p>





```input1
4
3 3
1 2 1
2 3 2
3 1 -1
3 3
1 2 1
2 3 1
3 1 -1
4 4
1 2 -1
2 3 -1
3 4 -1
4 1 -1
3 3
1 2 1
2 3 1
3 1 2
```




```output1
1 2 3 
1 1 1 
1 2 2 3 
-1
```


