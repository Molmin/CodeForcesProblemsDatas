## Description

<div><p><span class="tex-font-style-bf">The difference between the versions is in the costs of operations. Solution for one version won't work for another!</span></p><p>Alice has a grid of size $n \times m$, <span class="tex-font-style-bf">initially all its cells are colored white</span>. The cell on the intersection of $i$-th row and $j$-th column is denoted as $(i, j)$. Alice can do the following operations with this grid:</p><ul><li><p>Choose any subrectangle containing cell $(1, 1)$, and flip the colors of all its cells. (Flipping means changing its color from white to black or from black to white). </p><p><span class="tex-font-style-bf">This operation costs $1$ coin.</span></p></li><li><p>Choose any subrectangle containing cell $(n, 1)$, and flip the colors of all its cells. </p><p><span class="tex-font-style-bf">This operation costs $3$ coins.</span></p></li><li><p>Choose any subrectangle containing cell $(1, m)$, and flip the colors of all its cells. </p><p><span class="tex-font-style-bf">This operation costs $4$ coins.</span></p></li><li><p>Choose any subrectangle containing cell $(n, m)$, and flip the colors of all its cells. </p><p><span class="tex-font-style-bf">This operation costs $2$ coins.</span></p></li></ul> <p><span class="tex-font-style-bf">As a reminder, subrectangle is a set of all cells $(x, y)$ with $x_1 \le x \le x_2$, $y_1 \le y \le y_2$ for some $1 \le x_1 \le x_2 \le n$, $1 \le y_1 \le y_2 \le m$</span>.</p><p>Alice wants to obtain her favorite coloring with these operations. What's the smallest number of coins that she would have to spend? It can be shown that it's always possible to transform the initial grid into any other.</p></div><div class="input-specification"><p>The first line of the input contains $2$ integers $n, m$ ($1 \le n, m \le 500$) — the dimensions of the grid.</p><p>The $i$-th of the next $n$ lines contains a string $s_i$ of length $m$, consisting of letters <span class="tex-font-style-tt">W</span> and <span class="tex-font-style-tt">B</span>. The $j$-th character of string $s_i$ is <span class="tex-font-style-tt">W</span> if the cell $(i, j)$ is colored white in the favorite coloring of Alice, and <span class="tex-font-style-tt">B</span> if it's colored black.</p></div><div class="output-specification"><p>Output the smallest number of coins Alice would have to spend to achieve her favorite coloring.</p></div>

## Input

<p>The first line of the input contains $2$ integers $n, m$ ($1 \le n, m \le 500$) — the dimensions of the grid.</p><p>The $i$-th of the next $n$ lines contains a string $s_i$ of length $m$, consisting of letters <span class="tex-font-style-tt">W</span> and <span class="tex-font-style-tt">B</span>. The $j$-th character of string $s_i$ is <span class="tex-font-style-tt">W</span> if the cell $(i, j)$ is colored white in the favorite coloring of Alice, and <span class="tex-font-style-tt">B</span> if it's colored black.</p>

## Output

<p>Output the smallest number of coins Alice would have to spend to achieve her favorite coloring.</p>





```input1
3 3
WWW
WBB
WBB
```




```input2
10 15
WWWBBBWBBBBBWWW
BBBBWWWBBWWWBBB
BBBWWBWBBBWWWBB
BBWBWBBWWWBBWBW
BBBBWWWBBBWWWBB
BWBBWWBBBBBBWWW
WBWWBBBBWWBBBWW
WWBWWWWBBWWBWWW
BWBWWBWWWWWWBWB
BBBWBWBWBBBWWBW
```




```output1
2
```




```output2
68
```



## Note

<p>In the first sample, it's optimal to just apply the fourth operation once to the rectangle containing cells $(2, 2), (2, 3), (3, 2), (3, 3)$. This would cost $2$ coins.</p>
