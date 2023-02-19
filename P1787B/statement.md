## Description

<div><p>Given an integer $n$.</p><p>Consider all pairs of integer arrays $a$ and $p$ of the same length such that $n = \prod a_i^{p_i}$ (i.e. $a_1^{p_1}\cdot a_2^{p_2}\cdot\ldots$) ($a_i&gt;1;p_i&gt;0$) and $a_i$ is the product of some (possibly one) <span class="tex-font-style-bf">distinct</span> prime numbers.</p><p>For example, for $n = 28 = 2^2\cdot 7^1 = 4^1 \cdot 7^1$ the array pair $a = [2, 7]$, $p = [2, 1]$ is correct, but the pair of arrays $a = [4, 7]$, $p = [1, 1]$ is not, because $4=2^2$ is a product of non-distinct prime numbers.</p><p>Your task is to find the maximum value of $\sum a_i \cdot p_i$ (i.e. $a_1\cdot p_1 + a_2\cdot p_2 + \ldots$) over all possible pairs of arrays $a$ and $p$. Note that you do not need to minimize or maximize the length of the arrays.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$) — the number of test cases. </p><p>Each test case contains only one integer $n$ ($2 \le n \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print the maximum value of $\sum a_i \cdot p_i$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$) — the number of test cases. </p><p>Each test case contains only one integer $n$ ($2 \le n \le 10^9$).</p>

## Output

<p>For each test case, print the maximum value of $\sum a_i \cdot p_i$.</p>





```input1|2,4,6,8
7
100
10
864
130056192
1000000000
2
999999018
```




```output1
20
10
22
118
90
2
333333009
```



## Note

<p>In the first test case, $100 = 10^2$ so that $a = [10]$, $p = [2]$ when $\sum a_i \cdot p_i$ hits the maximum value $10\cdot 2 = 20$. Also, $a = [100]$, $p = [1]$ does not work since $100$ is not made of distinct prime factors.</p><p>In the second test case, we can consider $10$ as $10^1$, so $a = [10]$, $p = [1]$. Notice that when $10 = 2^1\cdot 5^1$, $\sum a_i \cdot p_i = 7$.</p>
