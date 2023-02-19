## Description

<div><p>Let's consider all integers in the range from $1$ to $n$ (inclusive).</p><p>Among all pairs of <span class="tex-font-style-bf">distinct</span> integers in this range, find the maximum possible greatest common divisor of integers in pair. Formally, find the maximum value of $\mathrm{gcd}(a, b)$, where $1 \leq a &lt; b \leq n$.</p><p>The greatest common divisor, $\mathrm{gcd}(a, b)$, of two positive integers $a$ and $b$ is the biggest integer that is a divisor of both $a$ and $b$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single integer $n$ ($2 \leq n \leq 10^6$).</p></div><div class="output-specification"><p>For each test case, output the maximum value of $\mathrm{gcd}(a, b)$ among all $1 \leq a &lt; b \leq n$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single integer $n$ ($2 \leq n \leq 10^6$).</p>

## Output

<p>For each test case, output the maximum value of $\mathrm{gcd}(a, b)$ among all $1 \leq a &lt; b \leq n$.</p>





```input1
2
3
5
```




```output1
1
2
```



## Note

<p>In the first test case, $\mathrm{gcd}(1, 2) = \mathrm{gcd}(2, 3) = \mathrm{gcd}(1, 3) = 1$.</p><p>In the second test case, $2$ is the maximum possible value, corresponding to $\mathrm{gcd}(2, 4)$.</p>
