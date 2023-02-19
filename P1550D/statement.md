## Description

<div><p>Let's call an integer array $a_1, a_2, \dots, a_n$ <span class="tex-font-style-it">good</span> if $a_i \neq i$ for each $i$.</p><p>Let $F(a)$ be the number of pairs $(i, j)$ ($1 \le i &lt; j \le n$) such that $a_i + a_j = i + j$.</p><p>Let's say that an array $a_1, a_2, \dots, a_n$ is <span class="tex-font-style-it">excellent</span> if: </p><ul> <li> $a$ is <span class="tex-font-style-it">good</span>; </li><li> $l \le a_i \le r$ for each $i$; </li><li> $F(a)$ is the maximum possible among all <span class="tex-font-style-it">good</span> arrays of size $n$. </li></ul><p>Given $n$, $l$ and $r$, calculate the number of <span class="tex-font-style-it">excellent</span> arrays modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. </p><p>The first and only line of each test case contains three integers $n$, $l$, and $r$ ($2 \le n \le 2 \cdot 10^5$; $-10^9 \le l \le 1$; $n \le r \le 10^9$).</p><p>It's guaranteed that the sum of $n$ doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the number of excellent arrays modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. </p><p>The first and only line of each test case contains three integers $n$, $l$, and $r$ ($2 \le n \le 2 \cdot 10^5$; $-10^9 \le l \le 1$; $n \le r \le 10^9$).</p><p>It's guaranteed that the sum of $n$ doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the number of excellent arrays modulo $10^9 + 7$.</p>





```input1
4
3 0 3
4 -3 5
42 -33 55
69 -42 146
```




```output1
4
10
143922563
698570404
```



## Note

<p>In the first test case, it can be proven that the maximum $F(a)$ among all <span class="tex-font-style-it">good</span> arrays $a$ is equal to $2$. The excellent arrays are: </p><ol> <li> $[2, 1, 2]$; </li><li> $[0, 3, 2]$; </li><li> $[2, 3, 2]$; </li><li> $[3, 0, 1]$. </li></ol>
