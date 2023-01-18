## Description

<div><p>You are given an undirected graph without self-loops or multiple edges which consists of $n$ vertices and $m$ edges. Also you are given three integers $n_1$, $n_2$ and $n_3$.</p><p>Can you label each vertex with one of three numbers <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span> or <span class="tex-font-style-tt">3</span> in such way, that: </p><ol> <li> Each vertex should be labeled by exactly one number <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span> or <span class="tex-font-style-tt">3</span>; </li><li> The total number of vertices with label <span class="tex-font-style-tt">1</span> should be equal to $n_1$; </li><li> The total number of vertices with label <span class="tex-font-style-tt">2</span> should be equal to $n_2$; </li><li> The total number of vertices with label <span class="tex-font-style-tt">3</span> should be equal to $n_3$; </li><li> $|col_u - col_v| = 1$ for each edge $(u, v)$, where $col_x$ is the label of vertex&nbsp;$x$. </li></ol><p>If there are multiple valid labelings, print any of them.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 5000$; $0 \le m \le 10^5$)&nbsp;— the number of vertices and edges in the graph.</p><p>The second line contains three integers $n_1$, $n_2$ and $n_3$ ($0 \le n_1, n_2, n_3 \le n$)&nbsp;— the number of labels <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span> and <span class="tex-font-style-tt">3</span>, respectively. It's guaranteed that $n_1 + n_2 + n_3 = n$.</p><p>Next $m$ lines contan description of edges: the $i$-th line contains two integers $u_i$, $v_i$ ($1 \le u_i, v_i \le n$; $u_i \neq v_i$) — the vertices the $i$-th edge connects. It's guaranteed that the graph doesn't contain self-loops or multiple edges.</p></div><div class="output-specification"><p>If valid labeling exists then print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. In the second line print string of length $n$ consisting of <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span> and <span class="tex-font-style-tt">3</span>. The $i$-th letter should be equal to the label of the $i$-th vertex.</p><p>If there is no valid labeling, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 5000$; $0 \le m \le 10^5$)&nbsp;— the number of vertices and edges in the graph.</p><p>The second line contains three integers $n_1$, $n_2$ and $n_3$ ($0 \le n_1, n_2, n_3 \le n$)&nbsp;— the number of labels <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span> and <span class="tex-font-style-tt">3</span>, respectively. It's guaranteed that $n_1 + n_2 + n_3 = n$.</p><p>Next $m$ lines contan description of edges: the $i$-th line contains two integers $u_i$, $v_i$ ($1 \le u_i, v_i \le n$; $u_i \neq v_i$) — the vertices the $i$-th edge connects. It's guaranteed that the graph doesn't contain self-loops or multiple edges.</p>

## Output

<p>If valid labeling exists then print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. In the second line print string of length $n$ consisting of <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span> and <span class="tex-font-style-tt">3</span>. The $i$-th letter should be equal to the label of the $i$-th vertex.</p><p>If there is no valid labeling, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
6 3
2 2 2
3 1
5 4
2 5
```




```input2
5 9
0 2 3
1 2
1 3
1 5
2 3
2 4
2 5
3 4
3 5
4 5
```




```output1
YES
112323
```




```output2
NO
```


