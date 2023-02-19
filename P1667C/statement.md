## Description

<div><p>You are given a board with $n$ rows and $n$ columns, numbered from $1$ to $n$. The intersection of the $a$-th row and $b$-th column is denoted by $(a, b)$.</p><p>A half-queen attacks cells in the same row, same column, and on one diagonal. More formally, a half-queen on $(a, b)$ attacks the cell $(c, d)$ if $a=c$ or $b=d$ or $a-b=c-d$.</p><center> <img class="tex-graphics" src="file://7a4B6z38.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The blue cells are under attack.</span> </center> What is the minimum number of half-queens that can be placed on that board so as to ensure that each square is attacked by at least one half-queen?<p>Construct an optimal solution.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$) — the size of the board.</p></div><div class="output-specification"><p>In the first line print a single integer $k$ — the minimum number of half-queens.</p><p>In each of the next $k$ lines print two integers $a_i$, $b_i$ ($1 \le a_i, b_i \le n$) — the position of the $i$-th half-queen.</p><p>If there are multiple solutions, print any.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$) — the size of the board.</p>

## Output

<p>In the first line print a single integer $k$ — the minimum number of half-queens.</p><p>In each of the next $k$ lines print two integers $a_i$, $b_i$ ($1 \le a_i, b_i \le n$) — the position of the $i$-th half-queen.</p><p>If there are multiple solutions, print any.</p>





```input1
1
```




```input2
2
```




```input3
3
```




```output1
1
1 1
```




```output2
1
1 1
```




```output3
2
1 1
1 2
```



## Note

<p>Example $1$: one half-queen is enough. Note: a half-queen on $(1, 1)$ attacks $(1, 1)$.</p><p>Example $2$: one half-queen is enough too. $(1, 2)$ or $(2, 1)$ would be wrong solutions, because a half-queen on $(1, 2)$ does not attack the cell $(2, 1)$ and vice versa. $(2, 2)$ is also a valid solution.</p><p>Example $3$: it is impossible to cover the board with one half queen. There are multiple solutions for $2$ half-queens; you can print any of them.</p>
