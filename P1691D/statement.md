## Description

<div><p>You are given an array $a$ of $n$ integers. You are asked to find out if the inequality $$\max(a_i, a_{i + 1}, \ldots, a_{j - 1}, a_{j}) \geq a_i + a_{i + 1} + \dots + a_{j - 1} + a_{j}$$ holds for all pairs of indices $(i, j)$, where $1 \leq i \leq j \leq n$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) &nbsp;— the size of the array.</p><p>The next line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, on a new line output "<span class="tex-font-style-tt">YES</span>" if the condition is satisfied for the given array, and "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each letter in any case (upper or lower).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) &nbsp;— the size of the array.</p><p>The next line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, on a new line output "<span class="tex-font-style-tt">YES</span>" if the condition is satisfied for the given array, and "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each letter in any case (upper or lower).</p>





```input1|2,3,6,7
3
4
-1 1 -1 2
5
-1 2 -3 2 -1
3
2 3 -1
```




```output1
YES
YES
NO
```



## Note

<p>In test cases $1$ and $2$, the given condition is satisfied for all $(i, j)$ pairs. </p><p>In test case $3$, the condition isn't satisfied for the pair $(1, 2)$ as $\max(2, 3) &lt; 2 + 3$.</p>
