## Description

<div><p>Given a sequence $a_1, a_2, \ldots, a_n$, find the minimum number of elements to remove from the sequence such that after the removal, the sum of every $2$ consecutive elements is even.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2,\dots,a_n$ ($1\leq a_i\leq10^9$) — elements of the sequence.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer — the minimum number of elements to remove from the sequence such that the sum of every $2$ consecutive elements is even.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2,\dots,a_n$ ($1\leq a_i\leq10^9$) — elements of the sequence.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print a single integer — the minimum number of elements to remove from the sequence such that the sum of every $2$ consecutive elements is even.</p>





```input1
2
5
2 4 3 6 8
6
3 5 9 7 1 3
```




```output1
1
0
```



## Note

<p>In the first test case, after removing $3$, the sequence becomes $[2,4,6,8]$. The pairs of consecutive elements are $\{[2, 4], [4, 6], [6, 8]\}$. Each consecutive pair has an even sum now. Hence, we only need to remove $1$ element to satisfy the condition asked.</p><p>In the second test case, each consecutive pair already has an even sum so we need not remove any element.</p>
