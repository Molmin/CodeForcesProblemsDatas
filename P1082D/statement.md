## Description

<div><p>Graph constructive problems are back! This time the graph you are asked to build should match the following properties.</p><p>The graph is connected if and only if there exists a path between every pair of vertices.</p><p>The diameter (aka "longest shortest path") of a connected undirected graph is the maximum number of edges in the <span class="tex-font-style-bf">shortest</span> path between any pair of its vertices.</p><p>The degree of a vertex is the number of edges incident to it.</p><p>Given a sequence of $n$ integers $a_1, a_2, \dots, a_n$ construct a <span class="tex-font-style-bf">connected undirected</span> graph of $n$ vertices such that:</p><ul> <li> the graph contains no self-loops and no multiple edges; </li><li> the degree $d_i$ of the $i$-th vertex doesn't exceed $a_i$ (i.e. $d_i \le a_i$); </li><li> the diameter of the graph is maximum possible. </li></ul><p>Output the resulting graph or report that no solution exists.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($3 \le n \le 500$) — the number of vertices in the graph.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n - 1$) — the upper limits to vertex degrees.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>" if no graph can be constructed under the given conditions.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" and the diameter of the resulting graph in the first line.</p><p>The second line should contain a single integer $m$ — the number of edges in the resulting graph.</p><p>The $i$-th of the next $m$ lines should contain two integers $v_i, u_i$ ($1 \le v_i, u_i \le n$, $v_i \neq u_i$) — the description of the $i$-th edge. The graph should contain no multiple edges — for each pair $(x, y)$ you output, you should output no more pairs $(x, y)$ or $(y, x)$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($3 \le n \le 500$) — the number of vertices in the graph.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n - 1$) — the upper limits to vertex degrees.</p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>" if no graph can be constructed under the given conditions.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" and the diameter of the resulting graph in the first line.</p><p>The second line should contain a single integer $m$ — the number of edges in the resulting graph.</p><p>The $i$-th of the next $m$ lines should contain two integers $v_i, u_i$ ($1 \le v_i, u_i \le n$, $v_i \neq u_i$) — the description of the $i$-th edge. The graph should contain no multiple edges — for each pair $(x, y)$ you output, you should output no more pairs $(x, y)$ or $(y, x)$.</p>





```input1
3
2 2 2
```




```input2
5
1 4 1 1 1
```




```input3
3
1 1 1
```




```output1
YES 2
2
1 2
2 3
```




```output2
YES 2
4
1 2
3 2
4 2
5 2
```




```output3
NO
```



## Note

<p>Here are the graphs for the first two example cases. Both have diameter of $2$.</p><center> <img class="tex-graphics" src="file://6jpndL9d.png" style="max-width: 100.0%;max-height: 100.0%;"> $d_1 = 1 \le a_1 = 2$<p>$d_2 = 2 \le a_2 = 2$</p><p>$d_3 = 1 \le a_3 = 2$ </p></center><center> <img class="tex-graphics" src="file://2HxoU9IP.png" style="max-width: 100.0%;max-height: 100.0%;"> $d_1 = 1 \le a_1 = 1$<p>$d_2 = 4 \le a_2 = 4$</p><p>$d_3 = 1 \le a_3 = 1$</p><p>$d_4 = 1 \le a_4 = 1$ </p></center>
