## Description

<div><p>You are given three integers $n$, $k$, $m$ and $m$ conditions $(l_1, r_1, x_1), (l_2, r_2, x_2), \dots, (l_m, r_m, x_m)$.</p><p>Calculate the number of distinct arrays $a$, consisting of $n$ integers such that: </p><ul> <li> $0 \le a_i &lt; 2^k$ for each $1 \le i \le n$; </li><li> bitwise AND of numbers $a[l_i] \&amp; a[l_i + 1] \&amp; \dots \&amp; a[r_i] = x_i$ for each $1 \le i \le m$. </li></ul><p>Two arrays $a$ and $b$ are considered different if there exists such a position $i$ that $a_i \neq b_i$. </p><p>The number can be pretty large so print it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $k$ and $m$ ($1 \le n \le 5 \cdot 10^5$, $1 \le k \le 30$, $0 \le m \le 5 \cdot 10^5$) — the length of the array $a$, the value such that all numbers in $a$ should be smaller than $2^k$ and the number of conditions, respectively.</p><p>Each of the next $m$ lines contains the description of a condition $l_i$, $r_i$ and $x_i$ ($1 \le l_i \le r_i \le n$, $0 \le x_i &lt; 2^k$) — the borders of the condition segment and the required bitwise AND value on it.</p></div><div class="output-specification"><p>Print a single integer — the number of distinct arrays $a$ that satisfy all the above conditions modulo $998244353$.</p></div>

## Input

<p>The first line contains three integers $n$, $k$ and $m$ ($1 \le n \le 5 \cdot 10^5$, $1 \le k \le 30$, $0 \le m \le 5 \cdot 10^5$) — the length of the array $a$, the value such that all numbers in $a$ should be smaller than $2^k$ and the number of conditions, respectively.</p><p>Each of the next $m$ lines contains the description of a condition $l_i$, $r_i$ and $x_i$ ($1 \le l_i \le r_i \le n$, $0 \le x_i &lt; 2^k$) — the borders of the condition segment and the required bitwise AND value on it.</p>

## Output

<p>Print a single integer — the number of distinct arrays $a$ that satisfy all the above conditions modulo $998244353$.</p>





```input1
4 3 2
1 3 3
3 4 6
```




```input2
5 2 3
1 3 2
2 5 0
3 3 3
```




```output1
3
```




```output2
33
```



## Note

<p>You can recall what is a bitwise AND operation <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">here</a>.</p><p>In the first example, the answer is the following arrays: $[3, 3, 7, 6]$, $[3, 7, 7, 6]$ and $[7, 3, 7, 6]$.</p>
