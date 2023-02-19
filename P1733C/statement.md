## Description

<div><p>You are given an array $a$ with $n$ non-negative integers. You can apply the following operation on it. </p><ul> <li> Choose two indices $l$ and $r$ ($1 \le l &lt; r \le n$). </li><li> If $a_l + a_r$ is odd, do $a_r := a_l$. If $a_l + a_r$ is even, do $a_l := a_r$. </li></ul><p>Find any sequence of at most $n$ operations that makes $a$ non-decreasing. It can be proven that it is always possible. Note that you do not have to minimize the number of operations.</p><p>An array $a_1, a_2, \ldots, a_n$ is non-decreasing if and only if $a_1 \le a_2 \le \ldots \le a_n$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>Each test case consists of two lines. The first line of each test case contains one integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) &nbsp;— the array itself.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer $m$ ($0 \le m \le n$), the number of operations, in the first line.</p><p>Then print $m$ lines. Each line must contain two integers $l_i, r_i$, which are the indices you chose in the $i$-th operation ($1 \le l_i &lt; r_i \le n$).</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>Each test case consists of two lines. The first line of each test case contains one integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) &nbsp;— the array itself.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case, print one integer $m$ ($0 \le m \le n$), the number of operations, in the first line.</p><p>Then print $m$ lines. Each line must contain two integers $l_i, r_i$, which are the indices you chose in the $i$-th operation ($1 \le l_i &lt; r_i \le n$).</p><p>If there are multiple solutions, print any of them.</p>





```input1|2,3,6,7
3
2
7 8
5
1 1000000000 3 0 5
1
0
```




```output1
0
2
3 4
1 2
0
```



## Note

<p>In the second test case, $a$ changes like this:</p><ul> <li> Select indices $3$ and $4$. $a_3 + a_4 = 3$ is odd, so do $a_4 := a_3$. $a = [1, 1000000000, 3, 3, 5]$ now. </li><li> Select indices $1$ and $2$. $a_1 + a_2 = 1000000001$ is odd, so do $a_2 := a_1$. $a = [1, 1, 3, 3, 5]$ now, and it is non-decreasing. </li></ul><p>In the first and third test cases, $a$ is already non-decreasing.</p>
