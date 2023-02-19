## Description

<div><p>You are given an array $a$ consisting of $n$ non-negative integers.</p><p>The <span class="tex-font-style-it">numbness</span> of a subarray $a_l, a_{l+1}, \ldots, a_r$ (for arbitrary $l \leq r$) is defined as $$\max(a_l, a_{l+1}, \ldots, a_r) \oplus (a_l \oplus a_{l+1} \oplus \ldots \oplus a_r),$$ where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>Find the maximum numbness over all subarrays.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer — the maximum numbness over all subarrays of the given array.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer — the maximum numbness over all subarrays of the given array.</p>





```input1|2,3
2
5
1 2 3 4 5
3
10 47 52
```




```output1
7
47
```



## Note

<p>For the first test case, for the subarray $[3, 4, 5]$, its maximum value is $5$. Hence, its numbness is $3 \oplus 4 \oplus 5 \oplus 5$ = $7$. This is the maximum possible numbness in this array.</p><p>In the second test case the subarray $[47, 52]$ provides the maximum numbness.</p>
