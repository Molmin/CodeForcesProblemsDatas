## Description

<div><p>You are given an array $a_1, a_2, \ldots, a_n$ of positive integers. A <span class="tex-font-style-it">good pair</span> is a pair of indices $(i, j)$ with $1 \leq i, j \leq n$ such that, for all $1 \leq k \leq n$, the following equality holds:</p><p>$$ |a_i - a_k| + |a_k - a_j| = |a_i - a_j|, $$ where $|x|$ denotes the absolute value of $x$.</p><p>Find a good pair. Note that $i$ can be equal to $j$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 1000$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$) — the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) where $a_i$ is the $i$-th element of the array.</p><p>The sum of $n$ for all test cases is at most $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line with two space-separated indices $i$ and $j$ which form a good pair of the array. The case $i=j$ is allowed. It can be shown that such a pair always exists. If there are multiple good pairs, print any of them.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 1000$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$) — the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) where $a_i$ is the $i$-th element of the array.</p><p>The sum of $n$ for all test cases is at most $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single line with two space-separated indices $i$ and $j$ which form a good pair of the array. The case $i=j$ is allowed. It can be shown that such a pair always exists. If there are multiple good pairs, print any of them.</p>





```input1
3
3
5 2 7
5
1 4 2 2 3
1
2
```




```output1
2 3
1 2
1 1
```



## Note

<p>In the first case, for $i = 2$ and $j = 3$ the equality holds true for all $k$: </p><ul> <li> $k = 1$: $|a_2 - a_1| + |a_1 - a_3| = |2 - 5| + |5 - 7| = 5 = |2 - 7| = |a_2-a_3|$, </li><li> $k = 2$: $|a_2 - a_2| + |a_2 - a_3| = |2 - 2| + |2 - 7| = 5 = |2 - 7| = |a_2-a_3|$, </li><li> $k = 3$: $|a_2 - a_3| + |a_3 - a_3| = |2 - 7| + |7 - 7| = 5 = |2 - 7| = |a_2-a_3|$. </li></ul>
