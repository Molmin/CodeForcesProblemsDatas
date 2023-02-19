## Description

<div><p>You are given an array $a$ of length $n$. You are asked to process $q$ queries of the following format: given integers $i$ and $x$, multiply $a_i$ by $x$.</p><p>After processing each query you need to output the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of all elements of the array $a$.</p><p>Since the answer can be too large, you are asked to output it modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains two integers — $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$) — the elements of the array $a$ before the changes.</p><p>The next $q$ lines contain queries in the following format: each line contains two integers $i$ and $x$ ($1 \le i \le n$, $1 \le x \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>Print $q$ lines: after processing each query output the GCD of all elements modulo $10^9+7$ on a separate line.</p></div>

## Input

<p>The first line contains two integers — $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$) — the elements of the array $a$ before the changes.</p><p>The next $q$ lines contain queries in the following format: each line contains two integers $i$ and $x$ ($1 \le i \le n$, $1 \le x \le 2 \cdot 10^5$).</p>

## Output

<p>Print $q$ lines: after processing each query output the GCD of all elements modulo $10^9+7$ on a separate line.</p>





```input1
4 3
1 6 8 12
1 12
2 3
3 3
```




```output1
2
2
6
```



## Note

<p>After the first query the array is $[12, 6, 8, 12]$, $\operatorname{gcd}(12, 6, 8, 12) = 2$.</p><p>After the second query — $[12, 18, 8, 12]$, $\operatorname{gcd}(12, 18, 8, 12) = 2$.</p><p>After the third query — $[12, 18, 24, 12]$, $\operatorname{gcd}(12, 18, 24, 12) = 6$.</p><p>Here the $\operatorname{gcd}$ function denotes the greatest common divisor.</p>
