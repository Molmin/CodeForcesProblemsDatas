## Description

<div><p>You are given a tree consisting of $n$ vertices. A tree is a connected undirected graph with $n-1$ edges. Each vertex $v$ of this tree has a color assigned to it ($a_v = 1$ if the vertex $v$ is white and $0$ if the vertex $v$ is black).</p><p>You have to solve the following problem for each vertex $v$: what is the maximum difference between the number of white and the number of black vertices you can obtain if you choose some subtree of the given tree that <span class="tex-font-style-bf">contains</span> the vertex $v$? The subtree of the tree is the connected subgraph of the given tree. More formally, if you choose the subtree that contains $cnt_w$ white vertices and $cnt_b$ black vertices, you have to maximize $cnt_w - cnt_b$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of vertices in the tree.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 1$), where $a_i$ is the color of the $i$-th vertex.</p><p>Each of the next $n-1$ lines describes an edge of the tree. Edge $i$ is denoted by two integers $u_i$ and $v_i$, the labels of vertices it connects $(1 \le u_i, v_i \le n, u_i \ne v_i$).</p><p>It is guaranteed that the given edges form a tree.</p></div><div class="output-specification"><p>Print $n$ integers $res_1, res_2, \dots, res_n$, where $res_i$ is the maximum possible difference between the number of white and black vertices in some subtree that contains the vertex $i$.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of vertices in the tree.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 1$), where $a_i$ is the color of the $i$-th vertex.</p><p>Each of the next $n-1$ lines describes an edge of the tree. Edge $i$ is denoted by two integers $u_i$ and $v_i$, the labels of vertices it connects $(1 \le u_i, v_i \le n, u_i \ne v_i$).</p><p>It is guaranteed that the given edges form a tree.</p>

## Output

<p>Print $n$ integers $res_1, res_2, \dots, res_n$, where $res_i$ is the maximum possible difference between the number of white and black vertices in some subtree that contains the vertex $i$.</p>





```input1
9
0 1 1 1 0 0 0 0 1
1 2
1 3
3 4
3 5
2 6
4 7
6 8
5 9
```




```input2
4
0 0 1 0
1 2
1 3
1 4
```




```output1
2 2 2 2 2 1 1 0 2
```




```output2
0 -1 1 -1
```



## Note

<p>The first example is shown below:</p><p><img class="tex-graphics" src="file://qe8q8x7z.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The black vertices have bold borders.</p><p>In the second example, the best subtree for vertices $2, 3$ and $4$ are vertices $2, 3$ and $4$ correspondingly. And the best subtree for the vertex $1$ is the subtree consisting of vertices $1$ and $3$.</p>
