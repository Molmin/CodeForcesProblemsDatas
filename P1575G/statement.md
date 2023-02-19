## Description

<div><p>Mr. Chanek has an array $a$ of $n$ integers. The prettiness value of $a$ is denoted as:</p><p>$$\sum_{i=1}^{n} {\sum_{j=1}^{n} {\gcd(a_i, a_j) \cdot \gcd(i, j)}}$$</p><p>where $\gcd(x, y)$ denotes the greatest common divisor (GCD) of integers $x$ and $y$.</p><p>In other words, the prettiness value of an array $a$ is the total sum of $\gcd(a_i, a_j) \cdot \gcd(i, j)$ for all pairs $(i, j)$.</p><p>Help Mr. Chanek find the prettiness value of $a$, and output the result modulo $10^9 + 7$!</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2 \leq n \leq 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^5$).</p></div><div class="output-specification"><p>Output an integer denoting the prettiness value of $a$ modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains an integer $n$ ($2 \leq n \leq 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^5$).</p>

## Output

<p>Output an integer denoting the prettiness value of $a$ modulo $10^9 + 7$.</p>





```input1
5
3 6 2 1 4
```




```output1
77
```


