## Description

<div><p>You are given an undirected tree of $n$ vertices. </p><p>Some vertices are colored one of the $k$ colors, some are uncolored. It is guaranteed that the tree contains at least one vertex of each of the $k$ colors. There might be no uncolored vertices.</p><p>You choose a subset of <span class="tex-font-style-bf">exactly $k - 1$ edges</span> and remove it from the tree. Tree falls apart into $k$ connected components. Let's call this subset of edges <span class="tex-font-style-it">nice</span> if none of the resulting components contain vertices of different colors.</p><p>How many <span class="tex-font-style-it">nice</span> subsets of edges are there in the given tree? Two subsets are considered different if there is some edge that is present in one subset and absent in the other.</p><p>The answer may be large, so print it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($2 \le n \le 3 \cdot 10^5$, $2 \le k \le n$) — the number of vertices in the tree and the number of colors, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le k$) — the colors of the vertices. $a_i = 0$ means that vertex $i$ is uncolored, any other value means the vertex $i$ is colored that color.</p><p>The $i$-th of the next $n - 1$ lines contains two integers $v_i$ and $u_i$ ($1 \le v_i, u_i \le n$, $v_i \ne u_i$) — the edges of the tree. It is guaranteed that the given edges form a tree. It is guaranteed that the tree contains at least one vertex of each of the $k$ colors. There might be no uncolored vertices.</p></div><div class="output-specification"><p>Print a single integer — the number of <span class="tex-font-style-it">nice</span> subsets of edges in the given tree. Two subsets are considered different if there is some edge that is present in one subset and absent in the other.</p><p>The answer may be large, so print it modulo $998244353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($2 \le n \le 3 \cdot 10^5$, $2 \le k \le n$) — the number of vertices in the tree and the number of colors, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le k$) — the colors of the vertices. $a_i = 0$ means that vertex $i$ is uncolored, any other value means the vertex $i$ is colored that color.</p><p>The $i$-th of the next $n - 1$ lines contains two integers $v_i$ and $u_i$ ($1 \le v_i, u_i \le n$, $v_i \ne u_i$) — the edges of the tree. It is guaranteed that the given edges form a tree. It is guaranteed that the tree contains at least one vertex of each of the $k$ colors. There might be no uncolored vertices.</p>

## Output

<p>Print a single integer — the number of <span class="tex-font-style-it">nice</span> subsets of edges in the given tree. Two subsets are considered different if there is some edge that is present in one subset and absent in the other.</p><p>The answer may be large, so print it modulo $998244353$.</p>





```input1
5 2
2 0 0 1 2
1 2
2 3
2 4
2 5
```




```input2
7 3
0 1 0 2 2 3 0
1 3
1 4
1 5
2 7
3 6
4 7
```




```output1
1
```




```output2
4
```



## Note

<p>Here is the tree from the first example:</p><center> <img class="tex-graphics" src="file://mYm5BBUt.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The only <span class="tex-font-style-it">nice</span> subset is edge $(2, 4)$. Removing it makes the tree fall apart into components $\{4\}$ and $\{1, 2, 3, 5\}$. The first component only includes a vertex of color $1$ and the second component includes only vertices of color $2$ and uncolored vertices.</p><p>Here is the tree from the second example:</p><center> <img class="tex-graphics" src="file://IUZ1pxXD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The <span class="tex-font-style-it">nice</span> subsets are $\{(1, 3), (4, 7)\}$, $\{(1, 3), (7, 2)\}$, $\{(3, 6), (4, 7)\}$ and $\{(3, 6), (7, 2)\}$.</p>
