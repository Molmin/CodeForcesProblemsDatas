## Description

<div><p>Madoka is a very strange girl, and therefore she suddenly wondered how many pairs of integers $(a, b)$ exist, where $1 \leq a, b \leq n$, for which $\frac{\operatorname{lcm}(a, b)}{\operatorname{gcd}(a, b)} \leq 3$.</p><p>In this problem, $\operatorname{gcd}(a, b)$ denotes <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor ">the greatest common divisor</a> of the numbers $a$ and $b$, and $\operatorname{lcm}(a, b)$ denotes <a href="https://en.wikipedia.org/wiki/Least_common_multiple ">the smallest common multiple</a> of the numbers $a$ and $b$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first and the only line of each test case contains the integer $n$ ($1 \le n \le 10^8$).</p></div><div class="output-specification"><p>For each test case output a single integer — the number of pairs of integers satisfying the condition.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first and the only line of each test case contains the integer $n$ ($1 \le n \le 10^8$).</p>

## Output

<p>For each test case output a single integer — the number of pairs of integers satisfying the condition.</p>





```input1|2,4,6
6
1
2
3
4
5
100000000
```




```output1
1
4
7
10
11
266666666
```



## Note

<p>For $n = 1$ there is exactly one pair of numbers&nbsp;— $(1, 1)$ and it fits.</p><p>For $n = 2$, there are only $4$ pairs&nbsp;— $(1, 1)$, $(1, 2)$, $(2, 1)$, $(2, 2)$ and they all fit.</p><p>For $n = 3$, all $9$ pair are suitable, except $(2, 3)$ and $(3, 2)$, since their $\operatorname{lcm}$ is $6$, and $\operatorname{gcd}$ is $1$, which doesn't fit the condition.</p>
