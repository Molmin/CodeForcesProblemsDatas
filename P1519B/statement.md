## Description

<div><p>There is a $n \times m$ grid. You are standing at cell $(1, 1)$ and your goal is to finish at cell $(n, m)$.</p><p>You can move to the neighboring cells to the right or down. In other words, suppose you are standing at cell $(x, y)$. You can: </p><ul> <li> move right to the cell $(x, y + 1)$&nbsp;— it costs $x$ burles; </li><li> move down to the cell $(x + 1, y)$&nbsp;— it costs $y$ burles. </li></ul><p>Can you reach cell $(n, m)$ spending <span class="tex-font-style-bf">exactly</span> $k$ burles?</p></div><div class="input-specification"><p>The first line contains the single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains three integers $n$, $m$, and $k$ ($1 \le n, m \le 100$; $0 \le k \le 10^4$)&nbsp;— the sizes of grid and the exact amount of money you need to spend.</p></div><div class="output-specification"><p>For each test case, if you can reach cell $(n, m)$ spending <span class="tex-font-style-bf">exactly</span> $k$ burles, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p></div>

## Input

<p>The first line contains the single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains three integers $n$, $m$, and $k$ ($1 \le n, m \le 100$; $0 \le k \le 10^4$)&nbsp;— the sizes of grid and the exact amount of money you need to spend.</p>

## Output

<p>For each test case, if you can reach cell $(n, m)$ spending <span class="tex-font-style-bf">exactly</span> $k$ burles, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p>





```input1
6
1 1 0
2 2 2
2 2 3
2 2 4
1 4 3
100 100 10000
```




```output1
YES
NO
YES
NO
YES
NO
```



## Note

<p>In the first test case, you are already in the final cell, so you spend $0$ burles.</p><p>In the second, third and fourth test cases, there are two paths from $(1, 1)$ to $(2, 2)$: $(1, 1)$ $\rightarrow$ $(1, 2)$ $\rightarrow$ $(2, 2)$ or $(1, 1)$ $\rightarrow$ $(2, 1)$ $\rightarrow$ $(2, 2)$. Both costs $1 + 2 = 3$ burles, so it's the only amount of money you can spend.</p><p>In the fifth test case, there is the only way from $(1, 1)$ to $(1, 4)$ and it costs $1 + 1 + 1 = 3$ burles.</p>
