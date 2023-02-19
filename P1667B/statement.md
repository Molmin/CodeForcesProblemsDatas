## Description

<div><p>You are given an array $a$ consisting of $n$ integers. You should divide $a$ into continuous non-empty subarrays (there are $2^{n-1}$ ways to do that).</p><p>Let $s=a_l+a_{l+1}+\ldots+a_r$. The value of a subarray $a_l, a_{l+1}, \ldots, a_r$ is: </p><ul> <li> $(r-l+1)$ if $s&gt;0$,</li><li> $0$ if $s=0$,</li><li> $-(r-l+1)$ if $s&lt;0$. </li></ul> What is the maximum sum of values you can get with a partition?</div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 5 \cdot 10^5$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($-10^9 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print a single integer — the maximum sum of values you can get with an optimal parition.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 5 \cdot 10^5$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($-10^9 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case print a single integer — the maximum sum of values you can get with an optimal parition.</p>





```input1
5
3
1 2 -3
4
0 -2 3 -4
5
-1 -2 3 -1 -1
6
-1 2 -3 4 -5 6
7
1 -1 -1 1 -1 -1 1
```




```output1
1
2
1
6
-1
```



## Note

<p>Test case $1$: one optimal partition is $[1, 2]$, $[-3]$. $1+2&gt;0$ so the value of $[1, 2]$ is $2$. $-3&lt;0$, so the value of $[-3]$ is $-1$. $2+(-1)=1$.</p><p>Test case $2$: the optimal partition is $[0, -2, 3]$, $[-4]$, and the sum of values is $3+(-1)=2$.</p>
