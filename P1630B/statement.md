## Description

<div><p>Given an array $a$ of $n$ integers, find a range of values $[x, y]$ ($x \le y$), and split $a$ into <span class="tex-font-style-bf">exactly</span> $k$ ($1 \le k \le n$) subarrays in such a way that:</p><ul> <li> Each subarray is formed by several continuous elements of $a$, that is, it is equal to $a_l, a_{l+1}, \ldots, a_r$ for some $l$ and $r$ ($1 \leq l \leq r \leq n$). </li><li> Each element from $a$ belongs to exactly one subarray. </li><li> In each subarray the number of elements inside the range $[x, y]$ (inclusive) is <span class="tex-font-style-bf">strictly greater</span> than the number of elements outside the range. An element with index $i$ is inside the range $[x, y]$ if and only if $x \le a_i \le y$. </li></ul> <p>Print any solution that minimizes $y - x$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 3 \cdot 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$) — the length of the array $a$ and the number of subarrays required in the partition.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$) where $a_i$ is the $i$-th element of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, print $k+1$ lines.</p><p>In the first line, print $x$ and $y$ — the limits of the found range.</p><p>Then print $k$ lines, the $i$-th should contain $l_i$ and $r_i$ ($1\leq l_i \leq r_i \leq n$) — the limits of the $i$-th subarray.</p><p>You can print the subarrays in any order.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 3 \cdot 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$) — the length of the array $a$ and the number of subarrays required in the partition.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$) where $a_i$ is the $i$-th element of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, print $k+1$ lines.</p><p>In the first line, print $x$ and $y$ — the limits of the found range.</p><p>Then print $k$ lines, the $i$-th should contain $l_i$ and $r_i$ ($1\leq l_i \leq r_i \leq n$) — the limits of the $i$-th subarray.</p><p>You can print the subarrays in any order.</p>





```input1
3
2 1
1 2
4 2
1 2 2 2
11 3
5 5 5 1 5 5 1 5 5 5 1
```




```output1
1 2
1 2
2 2
1 3
4 4
5 5
1 1
2 2
3 11
```



## Note

<p>In the first test, there should be only one subarray, which must be equal to the whole array. There are $2$ elements inside the range $[1, 2]$ and $0$ elements outside, if the chosen range is $[1, 1]$, there will be $1$ element inside ($a_1$) and $1$ element outside ($a_2$), and the answer will be invalid.</p><p>In the second test, it is possible to choose the range $[2, 2]$, and split the array in subarrays $(1, 3)$ and $(4, 4)$, in subarray $(1, 3)$ there are $2$ elements inside the range ($a_2$ and $a_3$) and $1$ element outside ($a_1$), in subarray $(4, 4)$ there is only $1$ element ($a_4$), and it is inside the range.</p><p>In the third test, it is possible to choose the range $[5, 5]$, and split the array in subarrays $(1, 4)$, $(5, 7)$ and $(8, 11)$, in the subarray $(1, 4)$ there are $3$ elements inside the range and $1$ element outside, in the subarray $(5, 7)$ there are $2$ elements inside and $1$ element outside and in the subarray $(8, 11)$ there are $3$ elements inside and $1$ element outside.</p>
