## Description

<div><p><span class="tex-font-style-bf">Note that the difference between easy and hard versions is that in hard version unavailable cells can become available again and in easy version can't. You can make hacks only if all versions are solved.</span></p><p>Ildar and Ivan are tired of chess, but they really like the chessboard, so they invented a new game. The field is a chessboard $2n \times 2m$: it has $2n$ rows, $2m$ columns, and the cell in row $i$ and column $j$ is colored white if $i+j$ is even, and is colored black otherwise.</p><p>The game proceeds as follows: Ildar marks some of the <span class="tex-font-style-bf">white</span> cells of the chessboard as <span class="tex-font-style-it">unavailable</span>, and asks Ivan to place $n \times m$ kings on the remaining <span class="tex-font-style-bf">white</span> cells in such way, so that there are no kings attacking each other. A king can attack another king if they are located in the adjacent cells, sharing an edge or a corner.</p><p>Ildar would like to explore different combinations of cells. Initially all cells are marked as available, and then he has $q$ queries. In each query he marks a cell as unavailable. After each query he would like to know whether it is possible to place the kings on the available cells in a desired way. Please help him!</p></div><div class="input-specification"><p>The first line of input contains three integers $n$, $m$, $q$ ($1 \leq n, m, q \leq 200\,000$)&nbsp;— the size of the board and the number of queries.</p><p>$q$ lines follow, each of them contains a description of a query: two integers $i$ and $j$, denoting a white cell $(i, j)$ on the board ($1 \leq i \leq 2n$, $1 \leq j \leq 2m$, $i + j$ is even) that becomes unavailable. It's guaranteed, that each cell $(i, j)$ appears in input at most once.</p></div><div class="output-specification"><p>Output $q$ lines, $i$-th line should contain answer for a board after $i$ queries of Ildar. This line should contain "<span class="tex-font-style-tt">YES</span>" if it is possible to place the kings on the available cells in the desired way, or "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line of input contains three integers $n$, $m$, $q$ ($1 \leq n, m, q \leq 200\,000$)&nbsp;— the size of the board and the number of queries.</p><p>$q$ lines follow, each of them contains a description of a query: two integers $i$ and $j$, denoting a white cell $(i, j)$ on the board ($1 \leq i \leq 2n$, $1 \leq j \leq 2m$, $i + j$ is even) that becomes unavailable. It's guaranteed, that each cell $(i, j)$ appears in input at most once.</p>

## Output

<p>Output $q$ lines, $i$-th line should contain answer for a board after $i$ queries of Ildar. This line should contain "<span class="tex-font-style-tt">YES</span>" if it is possible to place the kings on the available cells in the desired way, or "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
1 3 3
1 1
1 5
2 4
```




```input2
3 2 7
4 2
6 4
1 3
2 2
2 4
4 4
3 1
```




```output1
YES
YES
NO
```




```output2
YES
YES
NO
NO
NO
NO
NO
```



## Note

<p>In the first example case after the second query only cells $(1, 1)$ and $(1, 5)$ are unavailable. Then Ivan can place three kings on cells $(2, 2)$, $(2, 4)$ and $(2, 6)$.</p><p>After the third query three cells $(1, 1)$, $(1, 5)$ and $(2, 4)$ are unavailable, so there remain only 3 available cells: $(2, 2)$, $(1, 3)$ and $(2, 6)$. Ivan can not put 3 kings on those cells, because kings on cells $(2, 2)$ and $(1, 3)$ attack each other, since these cells share a corner.</p>
