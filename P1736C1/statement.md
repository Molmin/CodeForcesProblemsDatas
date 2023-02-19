## Description

<div><p><span class="tex-font-style-it">This is the easy version of this problem. In this version, we do not have queries. Note that we have multiple test cases in this version. You can make hacks only if both versions of the problem are solved.</span></p><p>An array $b$ of length $m$ is <span class="tex-font-style-it">good</span> if for all $i$ the $i$-th element is greater than or equal to $i$. In other words, $b$ is <span class="tex-font-style-it">good</span> if and only if $b_i \geq i$ for all $i$ ($1 \leq i \leq m$).</p><p>You are given an array $a$ consisting of $n$ positive integers. Find the number of pairs of indices $(l, r)$, where $1 \le l \le r \le n$, such that the array $[a_l, a_{l+1}, \ldots, a_r]$ is <span class="tex-font-style-it">good</span>.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 2 \cdot 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$), the length of the array $a$.</p><p>The second line of each test case contains $n$ space-separated integers $a_1,a_2,\ldots,a_n$ ($1 \leq a_i \leq n$), representing the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the number of suitable pairs of indices.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 2 \cdot 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$), the length of the array $a$.</p><p>The second line of each test case contains $n$ space-separated integers $a_1,a_2,\ldots,a_n$ ($1 \leq a_i \leq n$), representing the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the number of suitable pairs of indices.</p>





```input1|2,3,6,7
3
3
1 2 3
3
1 1 1
4
2 1 4 3
```




```output1
6
3
7
```



## Note

<p>In the first test case, all subarrays of $a$ are <span class="tex-font-style-it">good</span>, so all pairs are suitable.</p><p>In the second test case, the pairs $(1, 1)$, $(2, 2)$, and $(3, 3)$ are suitable. For example, when $(l, r) = (1, 2)$, the array $b=[1,1]$ is not <span class="tex-font-style-it">good</span> because $b_2 &lt; 2$.</p>
