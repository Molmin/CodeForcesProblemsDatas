## Description

<div><p>You are at the top left cell $(1, 1)$ of an $n \times m$ labyrinth. Your goal is to get to the bottom right cell $(n, m)$. You can only move right or down, one cell per step. Moving right from a cell $(x, y)$ takes you to the cell $(x, y + 1)$, while moving down takes you to the cell $(x + 1, y)$.</p><p>Some cells of the labyrinth contain rocks. When you move to a cell with rock, the rock is pushed to the next cell in the direction you're moving. If the next cell contains a rock, it gets pushed further, and so on.</p><p>The labyrinth is surrounded by impenetrable walls, thus any move that would put you or any rock outside of the labyrinth is illegal.</p><p>Count the number of different legal paths you can take from the start to the goal modulo $10^9 + 7$. Two paths are considered different if there is at least one cell that is visited in one path, but not visited in the other.</p></div><div class="input-specification"><p>The first line contains two integers $n, m$&nbsp;— dimensions of the labyrinth ($1 \leq n, m \leq 2000$).</p><p>Next $n$ lines describe the labyrinth. Each of these lines contains $m$ characters. The $j$-th character of the $i$-th of these lines is equal to "<span class="tex-font-style-tt">R</span>" if the cell $(i, j)$ contains a rock, or "<span class="tex-font-style-tt">.</span>" if the cell $(i, j)$ is empty.</p><p>It is guaranteed that the starting cell $(1, 1)$ is empty.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of different legal paths from $(1, 1)$ to $(n, m)$ modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains two integers $n, m$&nbsp;— dimensions of the labyrinth ($1 \leq n, m \leq 2000$).</p><p>Next $n$ lines describe the labyrinth. Each of these lines contains $m$ characters. The $j$-th character of the $i$-th of these lines is equal to "<span class="tex-font-style-tt">R</span>" if the cell $(i, j)$ contains a rock, or "<span class="tex-font-style-tt">.</span>" if the cell $(i, j)$ is empty.</p><p>It is guaranteed that the starting cell $(1, 1)$ is empty.</p>

## Output

<p>Print a single integer&nbsp;— the number of different legal paths from $(1, 1)$ to $(n, m)$ modulo $10^9 + 7$.</p>





```input1
1 1
.
```




```input2
2 3
...
..R
```




```input3
4 4
...R
.RR.
.RR.
R...
```




```output1
1
```




```output2
0
```




```output3
4
```



## Note

<p>In the first sample case we can't (and don't have to) move, hence the only path consists of a single cell $(1, 1)$.</p><p>In the second sample case the goal is blocked and is unreachable.</p><p>Illustrations for the third sample case can be found here: <a href="https://assets.codeforces.com/rounds/1225/index.html">https://assets.codeforces.com/rounds/1225/index.html</a></p>
