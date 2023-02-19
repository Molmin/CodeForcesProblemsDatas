## Description

<div><p>You are given two arrays $a$ and $b$ of length $n$. Array $a$ contains each <span class="tex-font-style-bf">odd</span> integer from $1$ to $2n$ in an arbitrary order, and array $b$ contains each <span class="tex-font-style-bf">even</span> integer from $1$ to $2n$ in an arbitrary order.</p><p>You can perform the following operation on those arrays: </p><ul> <li> choose one of the two arrays </li><li> pick an index $i$ from $1$ to $n-1$ </li><li> swap the $i$-th and the $(i+1)$-th elements of the chosen array </li></ul> Compute the minimum number of operations needed to make array $a$ lexicographically smaller than array $b$.<p>For two different arrays $x$ and $y$ of the same length $n$, we say that $x$ is lexicographically smaller than $y$ if in the first position where $x$ and $y$ differ, the array $x$ has a smaller element than the corresponding element in $y$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$).</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) — the length of the arrays.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 2n$, all $a_i$ are <span class="tex-font-style-bf">odd</span> and pairwise distinct) — array $a$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le 2n$, all $b_i$ are <span class="tex-font-style-bf">even</span> and pairwise distinct) — array $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer: the minimum number of operations needed to make array $a$ lexicographically smaller than array $b$.</p><p>We can show that an answer always exists.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$).</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) — the length of the arrays.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 2n$, all $a_i$ are <span class="tex-font-style-bf">odd</span> and pairwise distinct) — array $a$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le 2n$, all $b_i$ are <span class="tex-font-style-bf">even</span> and pairwise distinct) — array $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print one integer: the minimum number of operations needed to make array $a$ lexicographically smaller than array $b$.</p><p>We can show that an answer always exists.</p>





```input1
3
2
3 1
4 2
3
5 3 1
2 4 6
5
7 5 9 1 3
2 4 6 10 8
```




```output1
0
2
3
```



## Note

<p>In the first example, the array $a$ is already lexicographically smaller than array $b$, so no operations are required.</p><p>In the second example, we can swap $5$ and $3$ and then swap $2$ and $4$, which results in $[3, 5, 1]$ and $[4, 2, 6]$. Another correct way is to swap $3$ and $1$ and then swap $5$ and $1$, which results in $[1, 5, 3]$ and $[2, 4, 6]$. Yet another correct way is to swap $4$ and $6$ and then swap $2$ and $6$, which results in $[5, 3, 1]$ and $[6, 2, 4]$.</p>
