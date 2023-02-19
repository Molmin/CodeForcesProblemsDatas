## Description

<div><p>Suppose you have two points $p = (x_p, y_p)$ and $q = (x_q, y_q)$. Let's denote the Manhattan distance between them as $d(p, q) = |x_p - x_q| + |y_p - y_q|$.</p><p>Let's say that three points $p$, $q$, $r$ form a <span class="tex-font-style-it">bad</span> triple if $d(p, r) = d(p, q) + d(q, r)$.</p><p>Let's say that an array $b_1, b_2, \dots, b_m$ is <span class="tex-font-style-it">good</span> if it is impossible to choose three <span class="tex-font-style-bf">distinct</span> indices $i$, $j$, $k$ such that the points $(b_i, i)$, $(b_j, j)$ and $(b_k, k)$ form a bad triple.</p><p>You are given an array $a_1, a_2, \dots, a_n$. Calculate the number of <span class="tex-font-style-it">good</span> subarrays of $a$. A subarray of the array $a$ is the array $a_l, a_{l + 1}, \dots, a_r$ for some $1 \le l \le r \le n$.</p><p>Note that, according to the definition, subarrays of length $1$ and $2$ are <span class="tex-font-style-it">good</span>.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It's guaranteed that the sum of $n$ doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the number of <span class="tex-font-style-it">good</span> subarrays of array $a$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It's guaranteed that the sum of $n$ doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the number of <span class="tex-font-style-it">good</span> subarrays of array $a$.</p>





```input1
3
4
2 4 1 3
5
6 9 1 9 6
2
13 37
```




```output1
10
12
3
```



## Note

<p>In the first test case, it can be proven that any subarray of $a$ is <span class="tex-font-style-it">good</span>. For example, subarray $[a_2, a_3, a_4]$ is good since it contains only three elements and: </p><ul> <li> $d((a_2, 2), (a_4, 4)) = |4 - 3| + |2 - 4| = 3$ $&lt;$ $d((a_2, 2), (a_3, 3)) + d((a_3, 3), (a_4, 4)) = 3 + 1 + 2 + 1 = 7$; </li><li> $d((a_2, 2), (a_3, 3))$ $&lt;$ $d((a_2, 2), (a_4, 4)) + d((a_4, 4), (a_3, 3))$; </li><li> $d((a_3, 3), (a_4, 4))$ $&lt;$ $d((a_3, 3), (a_2, 2)) + d((a_2, 2), (a_4, 4))$; </li></ul><p>In the second test case, for example, subarray $[a_1, a_2, a_3, a_4]$ is <span class="tex-font-style-bf">not</span> good, since it contains a <span class="tex-font-style-it">bad</span> triple $(a_1, 1)$, $(a_2, 2)$, $(a_4, 4)$: </p><ul> <li> $d((a_1, 1), (a_4, 4)) = |6 - 9| + |1 - 4| = 6$; </li><li> $d((a_1, 1), (a_2, 2)) = |6 - 9| + |1 - 2| = 4$; </li><li> $d((a_2, 2), (a_4, 4)) = |9 - 9| + |2 - 4| = 2$; </li></ul><p>So, $d((a_1, 1), (a_4, 4)) = d((a_1, 1), (a_2, 2)) + d((a_2, 2), (a_4, 4))$.</p>
