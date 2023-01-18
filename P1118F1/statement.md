## Description

<div><p>You are given an undirected tree of $n$ vertices. </p><p>Some vertices are colored blue, some are colored red and some are uncolored. It is guaranteed that the tree contains at least one red vertex and at least one blue vertex.</p><p>You choose an edge and remove it from the tree. Tree falls apart into two connected components. Let's call an edge <span class="tex-font-style-it">nice</span> if neither of the resulting components contain vertices of both red and blue colors.</p><p>How many <span class="tex-font-style-it">nice</span> edges are there in the given tree?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 3 \cdot 10^5$) — the number of vertices in the tree.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2$) — the colors of the vertices. $a_i = 1$ means that vertex $i$ is colored red, $a_i = 2$ means that vertex $i$ is colored blue and $a_i = 0$ means that vertex $i$ is uncolored.</p><p>The $i$-th of the next $n - 1$ lines contains two integers $v_i$ and $u_i$ ($1 \le v_i, u_i \le n$, $v_i \ne u_i$) — the edges of the tree. It is guaranteed that the given edges form a tree. It is guaranteed that the tree contains at least one red vertex and at least one blue vertex.</p></div><div class="output-specification"><p>Print a single integer — the number of <span class="tex-font-style-it">nice</span> edges in the given tree.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 3 \cdot 10^5$) — the number of vertices in the tree.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2$) — the colors of the vertices. $a_i = 1$ means that vertex $i$ is colored red, $a_i = 2$ means that vertex $i$ is colored blue and $a_i = 0$ means that vertex $i$ is uncolored.</p><p>The $i$-th of the next $n - 1$ lines contains two integers $v_i$ and $u_i$ ($1 \le v_i, u_i \le n$, $v_i \ne u_i$) — the edges of the tree. It is guaranteed that the given edges form a tree. It is guaranteed that the tree contains at least one red vertex and at least one blue vertex.</p>

## Output

<p>Print a single integer — the number of <span class="tex-font-style-it">nice</span> edges in the given tree.</p>





```input1
5
2 0 0 1 2
1 2
2 3
2 4
2 5
```




```input2
5
1 0 0 0 2
1 2
2 3
3 4
4 5
```




```input3
3
1 1 2
2 3
1 3
```




```output1
1
```




```output2
4
```




```output3
0
```



## Note

<p>Here is the tree from the first example:</p><center> <img class="tex-graphics" src="file://FEjGCTTM.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The only <span class="tex-font-style-it">nice</span> edge is edge $(2, 4)$. Removing it makes the tree fall apart into components $\{4\}$ and $\{1, 2, 3, 5\}$. The first component only includes a red vertex and the second component includes blue vertices and uncolored vertices.</p><p>Here is the tree from the second example:</p><center> <img class="tex-graphics" src="file://uJBitvGT.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Every edge is <span class="tex-font-style-it">nice</span> in it.</p><p>Here is the tree from the third example:</p><center> <img class="tex-graphics" src="file://9xbRL7ME.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Edge $(1, 3)$ splits the into components $\{1\}$ and $\{3, 2\}$, the latter one includes both red and blue vertex, thus the edge isn't <span class="tex-font-style-it">nice</span>. Edge $(2, 3)$ splits the into components $\{1, 3\}$ and $\{2\}$, the former one includes both red and blue vertex, thus the edge also isn't <span class="tex-font-style-it">nice</span>. So the answer is 0.</p>
