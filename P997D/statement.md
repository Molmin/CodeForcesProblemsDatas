## Description

<div><p>Consider a tree (that is, an undirected connected graph without loops) $T_1$ and a tree $T_2$. Let's define their <span class="tex-font-style-it">cartesian product</span> $T_1 \times T_2$ in a following way.</p><p>Let $V$ be the set of vertices in $T_1$ and $U$ be the set of vertices in $T_2$.</p><p>Then the set of vertices of graph $T_1 \times T_2$ is $V \times U$, that is, a set of ordered pairs of vertices, where the first vertex in pair is from $V$ and the second&nbsp;— from $U$.</p><p>Let's draw the following edges:</p><ul><li> Between $(v, u_1)$ and $(v, u_2)$ there is an undirected edge, if $u_1$ and $u_2$ are adjacent in $U$. </li><li> Similarly, between $(v_1, u)$ and $(v_2, u)$ there is an undirected edge, if $v_1$ and $v_2$ are adjacent in $V$. </li></ul><p>Please see the notes section for the pictures of products of trees in the sample tests.</p><p>Let's examine the graph $T_1 \times T_2$. How much cycles (not necessarily simple) of length $k$ it contains? Since this number can be very large, print it modulo $998244353$.</p><p>The sequence of vertices $w_1$, $w_2$, ..., $w_k$, where $w_i \in V \times U$ called cycle, if any neighboring vertices are adjacent and $w_1$ is adjacent to $w_k$. Cycles that differ only by the cyclic shift or direction of traversal are still considered <span class="tex-font-style-bf">different</span>.</p></div><div class="input-specification"><p>First line of input contains three integers&nbsp;— $n_1$, $n_2$ and $k$ ($2 \le n_1, n_2 \le 4000$, $2 \le k \le 75$)&nbsp;— number of vertices in the first tree, number of vertices in the second tree and the cycle length respectively.</p><p>Then follow $n_1 - 1$ lines describing the first tree. Each of this lines contains two integers&nbsp;— $v_i, u_i$ ($1 \le v_i, u_i \le n_1$), which define edges of the first tree.</p><p>Then follow $n_2 - 1$ lines, which describe the second tree in the same format.</p><p>It is guaranteed, that given graphs are trees.</p></div><div class="output-specification"><p>Print one integer&nbsp;— number of cycles modulo $998244353$.</p></div>

## Input

<p>First line of input contains three integers&nbsp;— $n_1$, $n_2$ and $k$ ($2 \le n_1, n_2 \le 4000$, $2 \le k \le 75$)&nbsp;— number of vertices in the first tree, number of vertices in the second tree and the cycle length respectively.</p><p>Then follow $n_1 - 1$ lines describing the first tree. Each of this lines contains two integers&nbsp;— $v_i, u_i$ ($1 \le v_i, u_i \le n_1$), which define edges of the first tree.</p><p>Then follow $n_2 - 1$ lines, which describe the second tree in the same format.</p><p>It is guaranteed, that given graphs are trees.</p>

## Output

<p>Print one integer&nbsp;— number of cycles modulo $998244353$.</p>





```input1
2 2 2
1 2
1 2

```




```input2
2 2 4
1 2
1 2

```




```input3
2 3 4
1 2
1 2
1 3

```




```input4
4 2 2
1 2
1 3
1 4
1 2

```




```output1
8

```




```output2
32

```




```output3
70

```




```output4
20

```



## Note

<p>The following three pictures illustrate graph, which are products of the trees from sample tests.</p><p>In the first example, the list of cycles of length $2$ is as follows:</p><ul> <li> «AB», «BA» </li><li> «BC», «CB» </li><li> «AD», «DA» </li><li> «CD», «DC» </li></ul><center> <img class="tex-graphics" src="file://uDBQzHye.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://lB7t0WZI.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://uzHSxdan.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
