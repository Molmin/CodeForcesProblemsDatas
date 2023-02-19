## Description

<div><p>You are given two integers $n$ and $m$ and an array $a$ of $n$ integers. For each $1 \le i \le n$ it holds that $1 \le a_i \le m$.</p><p>Your task is to count the number of different arrays $b$ of length $n$ such that: </p><ul> <li> $1 \le b_i \le m$ for each $1 \le i \le n$, and </li><li> $\gcd(b_1,b_2,b_3,...,b_i) = a_i$ for each $1 \le i \le n$. </li></ul><p>Here $\gcd(a_1,a_2,\dots,a_i)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $a_1,a_2,\ldots,a_i$.</p><p>Since this number can be too large, print it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>Each test consist of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$, $1 \le m \le 10^9$) — the length of the array $a$ and the maximum possible value of the element.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le m$) — the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ across all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer — the number of different arrays satisfying the conditions above. Since this number can be large, print it modulo $998\,244\,353$.</p></div>

## Input

<p>Each test consist of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$, $1 \le m \le 10^9$) — the length of the array $a$ and the maximum possible value of the element.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le m$) — the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ across all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer — the number of different arrays satisfying the conditions above. Since this number can be large, print it modulo $998\,244\,353$.</p>





```input1|2,3,6,7,10,11
5
3 5
4 2 1
2 1
1 1
5 50
2 3 5 2 3
4 1000000000
60 30 1 1
2 1000000000
1000000000 2
```




```output1
3
1
0
595458194
200000000
```



## Note

<p>In the first test case, the possible arrays $b$ are: </p><ul> <li> $[4,2,1]$; </li><li> $[4,2,3]$; </li><li> $[4,2,5]$. </li></ul><p>In the second test case, the only array satisfying the demands is $[1,1]$.</p><p>In the third test case, it can be proven no such array exists.</p>
