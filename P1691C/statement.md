## Description

<div><p>You are given a binary string $s$ of length $n$.</p><p>Let's define $d_i$ as the number whose decimal representation is $s_i s_{i+1}$ (possibly, with a leading zero). We define $f(s)$ to be the sum of all the valid $d_i$. In other words, $f(s) = \sum\limits_{i=1}^{n-1} d_i$.</p><p>For example, for the string $s = 1011$: </p><ul> <li> $d_1 = 10$ (ten); </li><li> $d_2 = 01$ (one) </li><li> $d_3 = 11$ (eleven); </li><li> $f(s) = 10 + 01 + 11 = 22$. </li></ul><p>In one operation you can swap any two adjacent elements of the string. Find the minimum value of $f(s)$ that can be achieved if at most $k$ operations are allowed.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>First line of each test case contains two integers $n$ and $k$ ($2 \le n \le 10^5$, $0 \le k \le 10^9$)&nbsp;— the length of the string and the maximum number of operations allowed.</p><p>The second line of each test case contains the binary string $s$ of length $n$, consisting of only zeros and ones.</p><p>It is also given that sum of $n$ over all the test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print the minimum value of $f(s)$ you can obtain with at most $k$ operations.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>First line of each test case contains two integers $n$ and $k$ ($2 \le n \le 10^5$, $0 \le k \le 10^9$)&nbsp;— the length of the string and the maximum number of operations allowed.</p><p>The second line of each test case contains the binary string $s$ of length $n$, consisting of only zeros and ones.</p><p>It is also given that sum of $n$ over all the test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case, print the minimum value of $f(s)$ you can obtain with at most $k$ operations.</p>





```input1
3
4 0
1010
7 1
0010100
5 2
00110
```




```output1
21
22
12
```



## Note

<ul> <li> For the first example, you can't do any operation so the optimal string is $s$ itself. $f(s) = f(1010) = 10 + 01 + 10 = 21$. </li><li> For the second example, one of the optimal strings you can obtain is "<span class="tex-font-style-tt">0011000</span>". The string has an $f$ value of $22$. </li><li> For the third example, one of the optimal strings you can obtain is "<span class="tex-font-style-tt">00011</span>". The string has an $f$ value of $12$. </li></ul>
