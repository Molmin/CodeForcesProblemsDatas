## Description

<div><p>You are given two positive integer sequences $a_1, \ldots, a_n$ and $b_1, \ldots, b_m$. For each $j = 1, \ldots, m$ find the greatest common divisor of $a_1 + b_j, \ldots, a_n + b_j$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \leq n, m \leq 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, \ldots, a_n$ ($1 \leq a_i \leq 10^{18})$.</p><p>The third line contains $m$ integers $b_1, \ldots, b_m$ ($1 \leq b_j \leq 10^{18})$.</p></div><div class="output-specification"><p>Print $m$ integers. The $j$-th of them should be equal to GCD$(a_1 + b_j, \ldots, a_n + b_j)$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \leq n, m \leq 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, \ldots, a_n$ ($1 \leq a_i \leq 10^{18})$.</p><p>The third line contains $m$ integers $b_1, \ldots, b_m$ ($1 \leq b_j \leq 10^{18})$.</p>

## Output

<p>Print $m$ integers. The $j$-th of them should be equal to GCD$(a_1 + b_j, \ldots, a_n + b_j)$.</p>





```input1
4 4
1 25 121 169
1 2 7 23
```




```output1
2 3 8 24
```


