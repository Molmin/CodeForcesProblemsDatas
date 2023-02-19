## Description

<div><p>You are given a positive integer $n$. You have to find $4$ <span class="tex-font-style-bf">positive</span> integers $a, b, c, d$ such that</p><ul> <li> $a + b + c + d = n$, and</li><li> $\gcd(a, b) = \operatorname{lcm}(c, d)$.</li></ul><p>If there are several possible answers you can output any of them. It is possible to show that the answer always exists.</p><p>In this problem $\gcd(a, b)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a> of $a$ and $b$, and $\operatorname{lcm}(c, d)$ denotes the <a href="https://en.wikipedia.org/wiki/Least_common_multiple">least common multiple</a> of $c$ and $d$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>Each test case contains a single line with integer $n$ ($4 \le n \le 10^9$)&nbsp;— the sum of $a$, $b$, $c$, and $d$.</p></div><div class="output-specification"><p>For each test case output $4$ <span class="tex-font-style-bf">positive</span> integers $a$, $b$, $c$, $d$ such that $a + b + c + d = n$ and $\gcd(a, b) = \operatorname{lcm}(c, d)$.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>Each test case contains a single line with integer $n$ ($4 \le n \le 10^9$)&nbsp;— the sum of $a$, $b$, $c$, and $d$.</p>

## Output

<p>For each test case output $4$ <span class="tex-font-style-bf">positive</span> integers $a$, $b$, $c$, $d$ such that $a + b + c + d = n$ and $\gcd(a, b) = \operatorname{lcm}(c, d)$.</p>





```input1
5
4
7
8
9
10
```




```output1
1 1 1 1
2 2 2 1
2 2 2 2
2 4 2 1
3 5 1 1
```



## Note

<p>In the first test case $\gcd(1, 1) = \operatorname{lcm}(1, 1) = 1$, $1 + 1 + 1 + 1 = 4$.</p><p>In the second test case $\gcd(2, 2) = \operatorname{lcm}(2, 1) = 2$, $2 + 2 + 2 + 1 = 7$.</p><p>In the third test case $\gcd(2, 2) = \operatorname{lcm}(2, 2) = 2$, $2 + 2 + 2 + 2 = 8$.</p><p>In the fourth test case $\gcd(2, 4) = \operatorname{lcm}(2, 1) = 2$, $2 + 4 + 2 + 1 = 9$.</p><p>In the fifth test case $\gcd(3, 5) = \operatorname{lcm}(1, 1) = 1$, $3 + 5 + 1 + 1 = 10$. </p>
