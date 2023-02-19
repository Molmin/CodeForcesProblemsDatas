## Description

<div><p>You are given an array $a$ of length $n$. We define the <span class="tex-font-style-bf">equality</span> of the array as the number of indices $1 \le i \le n - 1$ such that $a_i = a_{i + 1}$. We are allowed to do the following operation:</p><ul> <li> Select two integers $i$ and $x$ such that $1 \le i \le n - 1$ and $1 \le x \le 10^9$. Then, set $a_i$ and $a_{i + 1}$ to be equal to $x$. </li></ul><p>Find the minimum number of operations needed such that the equality of the array is less than or equal to $1$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 2 \cdot 10 ^ 5$) — the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) — elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10 ^ 5$</p></div><div class="output-specification"><p>For each test case, print the minimum number of operations needed.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 2 \cdot 10 ^ 5$) — the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) — elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10 ^ 5$</p>

## Output

<p>For each test case, print the minimum number of operations needed.</p>





```input1|2,3,6,7
4
5
1 1 1 1 1
5
2 1 1 1 2
6
1 1 2 3 3 4
6
1 2 1 4 5 4
```




```output1
2
1
2
0
```



## Note

<p>In the first test case, we can select $i=2$ and $x=2$ to form $[1, 2, 2, 1, 1]$. Then, we can select $i=3$ and $x=3$ to form $[1, 2, 3, 3, 1]$.</p><p>In the second test case, we can select $i=3$ and $x=100$ to form $[2, 1, 100, 100, 2]$.</p>
