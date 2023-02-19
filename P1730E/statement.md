## Description

<div><p>You are given an array $a_1, a_2, \ldots, a_n$ of positive integers.</p><p>Find the number of pairs of indices $(l, r)$, where $1 \le l \le r \le n$, that pass the check. The check is performed in the following manner: </p><ol> <li> The minimum and maximum numbers are found among $a_l, a_{l+1}, \ldots, a_r$. </li><li> The check is passed if the maximum number is divisible by the minimum number. </li></ol></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10$) — the number of test cases. Then the test cases follow.</p><p>Each test case consists of two lines.</p><p>The first line contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the size of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer — the number of pairs of indices that pass the check.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10$) — the number of test cases. Then the test cases follow.</p><p>Each test case consists of two lines.</p><p>The first line contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the size of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer — the number of pairs of indices that pass the check.</p>





```input1|2,3,6,7,10,11
6
1
1
2
2 4
2
2 3
4
2 4 7 14
7
16 5 18 7 7 12 14
6
16 14 2 6 16 2
```




```output1
1
3
2
7
10
19
```



## Note

<p>Below $x \mid y$ denotes that $y$ is divisible by $x$.</p><p>In the first test case, there is one pair $(1, 1)$, the maximum for this pair is $1$, the minimum is also $1$, $1 \mid 1$, so the check is passed, and the answer is $1$.</p><p>In the second test case, there are $3$ segments: </p><ul> <li> $(1, 1)$: the maximum is $2$, the minimum is $2$, $2 \mid 2$, so the check is passed. </li><li> $(1, 2)$: the maximum is $4$, the minimum is $2$, $2 \mid 4$, so the check is passed. </li><li> $(2, 2)$: the maximum is $4$, the minimum is $4$, $4 \mid 4$, so the check is passed. </li></ul><p>In the third test case, there are $3$ segments: </p><ul> <li> $(1, 1)$: the maximum is $2$, the minimum is $2$, $2 \mid 2$, so the check is passed. </li><li> $(1, 2)$: the maximum is $3$, the minimum is $2$, $3$ isn't divisible by $2$, so the check is failed. </li><li> $(2, 2)$: the maximum is $3$, the minimum is $3$, $3 \mid 3$, so the check is passed. </li></ul>
