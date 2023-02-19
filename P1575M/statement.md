## Description

<div><p>Mr. Chanek's city can be represented as a plane. He wants to build a housing complex in the city.</p><p>There are some telephone poles on the plane, which is represented by a grid $a$ of size $(n + 1) \times (m + 1)$. There is a telephone pole at $(x, y)$ if $a_{x, y} = 1$.</p><p>For each point $(x, y)$, define $S(x, y)$ as the square of the Euclidean distance between the nearest pole and $(x, y)$. Formally, the square of the Euclidean distance between two points $(x_1, y_1)$ and $(x_2, y_2)$ is $(x_2 - x_1)^2 + (y_2 - y_1)^2$.</p><p>To optimize the building plan, the project supervisor asks you the sum of all $S(x, y)$ for each $0 \leq x \leq n$ and $0 \leq y \leq m$. Help him by finding the value of $\sum_{x=0}^{n} {\sum_{y=0}^{m} {S(x, y)}}$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($0 \leq n, m &lt; 2000$) — the size of the grid.</p><p>Then $(n + 1)$ lines follow, each containing $(m + 1)$ integers $a_{i, j}$ ($0 \leq a_{i, j} \leq 1$) — the grid denoting the positions of telephone poles in the plane. There is at least one telephone pole in the given grid.</p></div><div class="output-specification"><p>Output an integer denoting the value of $\sum_{x=0}^{n} {\sum_{y=0}^{m} {S(x, y)}}$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($0 \leq n, m &lt; 2000$) — the size of the grid.</p><p>Then $(n + 1)$ lines follow, each containing $(m + 1)$ integers $a_{i, j}$ ($0 \leq a_{i, j} \leq 1$) — the grid denoting the positions of telephone poles in the plane. There is at least one telephone pole in the given grid.</p>

## Output

<p>Output an integer denoting the value of $\sum_{x=0}^{n} {\sum_{y=0}^{m} {S(x, y)}}$.</p>





```input1
2 2
101
000
000
```




```input2
5 4
10010
00000
01000
00001
00100
00010
```




```output1
18
```




```output2
36
```



## Note

<center> <img class="tex-graphics" src="file://7BuprYUj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the first example, the nearest telephone pole for the points $(0,0)$, $(1,0)$, $(2,0)$, $(0,1)$, $(1,1)$, and $(2,1)$ is at $(0, 0)$. While the nearest telephone pole for the points $(0, 2)$, $(1,2)$, and $(2,2)$ is at $(0, 2)$. Thus, $\sum_{x=0}^{n} {\sum_{y=0}^{m} {S(x, y)}} = (0 + 1 + 4) + (1 + 2 + 5) + (0 + 1 + 4) = 18$.</p>
