## Description

<div><p>You are given two arrays of integers $a_1, a_2, \ldots, a_n$ and $b_1, b_2, \ldots, b_m$.</p><p>You need to insert all elements of $b$ into $a$ in an arbitrary way. As a result you will get an array $c_1, c_2, \ldots, c_{n+m}$ of size $n + m$.</p><p>Note that you are not allowed to change the order of elements in $a$, while you can insert elements of $b$ at arbitrary positions. They can be inserted at the beginning, between any elements of $a$, or at the end. Moreover, elements of $b$ can appear in the resulting array in any order.</p><p>What is the minimum possible number of inversions in the resulting array $c$? Recall that an inversion is a pair of indices $(i, j)$ such that $i &lt; j$ and $c_i &gt; c_j$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 10^6$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>The third line of each test case contains $m$ integers $b_1, b_2, \ldots, b_m$ ($1 \leq b_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ for all tests cases in one input doesn't exceed $10^6$. The sum of $m$ for all tests cases doesn't exceed $10^6$ as well.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the minimum possible number of inversions in the resulting array $c$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 10^6$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>The third line of each test case contains $m$ integers $b_1, b_2, \ldots, b_m$ ($1 \leq b_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ for all tests cases in one input doesn't exceed $10^6$. The sum of $m$ for all tests cases doesn't exceed $10^6$ as well.</p>

## Output

<p>For each test case, print one integer&nbsp;— the minimum possible number of inversions in the resulting array $c$.</p>





```input1
3
3 4
1 2 3
4 3 2 1
3 3
3 2 1
1 2 3
5 4
1 3 5 3 1
4 3 6 1
```




```output1
0
4
6
```



## Note

<p>Below is given the solution to get the optimal answer for each of the example test cases (elements of $a$ are underscored).</p><ul> <li> In the first test case, $c = [\underline{1}, 1, \underline{2}, 2, \underline{3}, 3, 4]$. </li><li> In the second test case, $c = [1, 2, \underline{3}, \underline{2}, \underline{1}, 3]$. </li><li> In the third test case, $c = [\underline{1}, 1, 3, \underline{3}, \underline{5}, \underline{3}, \underline{1}, 4, 6]$. </li></ul>
