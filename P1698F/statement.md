## Description

<div><p>There is an array $a$ of length $n$. You may perform the following operation on it:</p><ul> <li> Choose two indices $l$ and $r$ where $1 \le l \le r \le n$ and $a_l = a_r$. Then, reverse the subsegment from the $l$-th to the $r$-th element, i.&nbsp;e. set $[a_l, a_{l + 1}, \ldots, a_{r - 1}, a_r]$ to $[a_r, a_{r-1}, \ldots, a_{l+1}, a_l]$. </li></ul><p>You are also given another array $b$ of length $n$ which is a permutation of $a$. Find a sequence of at most $n^2$ operations that transforms array $a$ into $b$, or report that no such sequence exists.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 500$)&nbsp;— the length of array $a$ and $b$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— elements of the array $a$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le n$)&nbsp;— elements of the array $b$.</p><p>It is guaranteed that $b$ is a permutation of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $500$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">NO</span>" (without quotes) if it is impossible to turn $a$ into $b$ using at most $n^2$ operations.</p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>" (without quotes). Then output an integer $k$ ($0 \leq k \leq n^2$) denoting the number of operations you will perform. Note that you don't have to minimize the number of operations.</p><p>Afterwards, output $k$ lines. The $i$-th line should contain two integers $l_i$ and $r_i$ ($1 \leq l_i \leq r_i \leq n$)&nbsp;— the left and right indices for the $i$-th operation.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p><p>If there are multiple possible sequences of operations, you may output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 500$)&nbsp;— the length of array $a$ and $b$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— elements of the array $a$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le n$)&nbsp;— elements of the array $b$.</p><p>It is guaranteed that $b$ is a permutation of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $500$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">NO</span>" (without quotes) if it is impossible to turn $a$ into $b$ using at most $n^2$ operations.</p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>" (without quotes). Then output an integer $k$ ($0 \leq k \leq n^2$) denoting the number of operations you will perform. Note that you don't have to minimize the number of operations.</p><p>Afterwards, output $k$ lines. The $i$-th line should contain two integers $l_i$ and $r_i$ ($1 \leq l_i \leq r_i \leq n$)&nbsp;— the left and right indices for the $i$-th operation.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p><p>If there are multiple possible sequences of operations, you may output any of them.</p>





```input1|2,3,4,8,9,10,14,15,16
5
8
1 2 4 3 1 2 1 1
1 1 3 4 2 1 2 1
7
1 2 3 1 3 2 3
1 3 2 3 1 2 3
3
1 1 2
1 2 1
2
1 2
2 1
1
1
1
```




```output1
YES
2
5 8
1 6
YES
2
1 4
3 6
NO
NO
YES
0
```



## Note

<p>In the first test case, we can perform the following operations: $$[1,2,4,3,1,2,1,1] \xrightarrow[l=5,\,r=8]{} [1,2,4,3,1,1,2,1] \xrightarrow[l=1,\,r=6]{} [1,1,3,4,2,1,2,1].$$</p><p>In the second test case, we can perform the following operations: $$[1,2,3,1,3,2,3] \xrightarrow[l=1,\,r=4]{} [1,3,2,1,3,2,3] \xrightarrow[l=3,\,r=6]{} [1,3,2,3,1,2,3].$$</p><p>It can be proven that it is impossible to turn $a$ into $b$ in the third and fourth test cases.</p>
