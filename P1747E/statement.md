## Description

<div><p>For given integers $n$ and $m$, let's call a pair of arrays $a$ and $b$ of integers <span class="tex-font-style-bf">good</span>, if they satisfy the following conditions: </p><ul> <li> $a$ and $b$ have the same length, let their length be $k$.</li><li> $k \ge 2$ and $a_1 = 0, a_k = n, b_1 = 0, b_k = m$.</li><li> For each $1 &lt; i \le k$ the following holds: $a_i \geq a_{i - 1}$, $b_i \geq b_{i - 1}$, and $a_i + b_i \neq a_{i - 1} + b_{i - 1}$.</li></ul><p>Find the sum of $|a|$ over all good pairs of arrays $(a,b)$. Since the answer can be very large, output it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t (1 \leq t \leq 10^4)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $m$ $(1 \leq n, m \leq 5 \cdot 10^6)$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^6$ and the sum of $m$ over all test cases does not exceed $5 \cdot 10^6$.</p></div><div class="output-specification"><p>For each test case, output a single integer &nbsp;— the sum of $|a|$ over all good pairs of arrays $(a,b)$ modulo $10^9 + 7$.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t (1 \leq t \leq 10^4)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $m$ $(1 \leq n, m \leq 5 \cdot 10^6)$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^6$ and the sum of $m$ over all test cases does not exceed $5 \cdot 10^6$.</p>

## Output

<p>For each test case, output a single integer &nbsp;— the sum of $|a|$ over all good pairs of arrays $(a,b)$ modulo $10^9 + 7$.</p>





```input1|2,4
4
1 1
1 2
2 2
100 100
```




```output1
8
26
101
886336572
```



## Note

<p>In the <span class="tex-font-style-bf">first testcase</span>, the good pairs of arrays are </p><ul> <li> $([0, 1], [0, 1])$, length = $2$. </li><li> $([0, 1, 1], [0, 0, 1])$, length = $3$. </li><li> $([0, 0, 1], [0, 1, 1])$, length = $3$. </li></ul><p>Hence the sum of the lengths would be ${2 + 3 + 3} = 8$.</p>
