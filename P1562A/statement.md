## Description

<div><p>You are given two integers $l$ and $r$, $l\le r$. Find the largest possible value of $a \bmod b$ over all pairs $(a, b)$ of integers for which $r\ge a \ge b \ge l$.</p><p>As a reminder, $a \bmod b$ is a remainder we get when dividing $a$ by $b$. For example, $26 \bmod 8 = 2$.</p></div><div class="input-specification"><p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ $(1\le t\le 10^4)$, denoting the number of test cases. Description of the test cases follows.</p><p>The only line of each test case contains two integers $l$, $r$ ($1\le l \le r \le 10^9$).</p></div><div class="output-specification"><p>For every test case, output the largest possible value of $a \bmod b$ over all pairs $(a, b)$ of integers for which $r\ge a \ge b \ge l$.</p></div>

## Input

<p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ $(1\le t\le 10^4)$, denoting the number of test cases. Description of the test cases follows.</p><p>The only line of each test case contains two integers $l$, $r$ ($1\le l \le r \le 10^9$).</p>

## Output

<p>For every test case, output the largest possible value of $a \bmod b$ over all pairs $(a, b)$ of integers for which $r\ge a \ge b \ge l$.</p>





```input1
4
1 1
999999999 1000000000
8 26
1 999999999
```




```output1
0
1
12
499999999
```



## Note

<p>In the first test case, the only allowed pair is $(a, b) = (1, 1)$, for which $a \bmod b = 1 \bmod 1 = 0$.</p><p>In the second test case, the optimal choice is pair $(a, b) = (1000000000, 999999999)$, for which $a \bmod b = 1$.</p>
