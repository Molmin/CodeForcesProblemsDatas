## Description

<div><p>Given a positive integer $n$. Find three <span class="tex-font-style-bf">distinct</span> positive integers $a$, $b$, $c$ such that $a + b + c = n$ and $\operatorname{gcd}(a, b) = c$, where $\operatorname{gcd}(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $x$ and $y$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first and only line of each test case contains a single integer $n$ ($10 \le n \le 10^9$).</p></div><div class="output-specification"><p>For each test case, output three <span class="tex-font-style-bf">distinct</span> positive integers $a$, $b$, $c$ satisfying the requirements. If there are multiple solutions, you can print any. We can show that an answer always exists.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first and only line of each test case contains a single integer $n$ ($10 \le n \le 10^9$).</p>

## Output

<p>For each test case, output three <span class="tex-font-style-bf">distinct</span> positive integers $a$, $b$, $c$ satisfying the requirements. If there are multiple solutions, you can print any. We can show that an answer always exists.</p>





```input1
6
18
63
73
91
438
122690412
```




```output1
6 9 3
21 39 3
29 43 1
49 35 7
146 219 73
28622 122661788 2
```



## Note

<p>In the first test case, $6 + 9 + 3 = 18$ and $\operatorname{gcd}(6, 9) = 3$.</p><p>In the second test case, $21 + 39 + 3 = 63$ and $\operatorname{gcd}(21, 39) = 3$.</p><p>In the third test case, $29 + 43 + 1 = 73$ and $\operatorname{gcd}(29, 43) = 1$.</p>
