## Description

<div><p>Mark is cleaning a row of $n$ rooms. The $i$-th room has a nonnegative dust level $a_i$. He has a magical cleaning machine that can do the following three-step operation. </p><ul> <li> Select two indices $i&lt;j$ such that the dust levels $a_i$, $a_{i+1}$, $\dots$, $a_{j-1}$ are all strictly greater than $0$. </li><li> Set $a_i$ to $a_i-1$. </li><li> Set $a_j$ to $a_j+1$. </li></ul> Mark's goal is to make $a_1 = a_2 = \ldots = a_{n-1} = 0$ so that he can nicely sweep the $n$-th room. Determine the minimum number of operations needed to reach his goal.</div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\leq t\leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2\leq n\leq 2\cdot 10^5$) — the number of rooms.</p><p>The second line of each test case contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($0\leq a_i\leq 10^9$) — the dust level of each room.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a line containing a single integer — the minimum number of operations. It can be proven that there is a sequence of operations that meets the goal.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\leq t\leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2\leq n\leq 2\cdot 10^5$) — the number of rooms.</p><p>The second line of each test case contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($0\leq a_i\leq 10^9$) — the dust level of each room.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, print a line containing a single integer — the minimum number of operations. It can be proven that there is a sequence of operations that meets the goal.</p>





```input1|2,3,6,7
4
3
2 0 0
5
0 2 0 2 0
6
2 0 3 0 4 6
4
0 0 0 10
```




```output1
3
5
11
0
```



## Note

<p>In the first case, one possible sequence of operations is as follows. </p><ul> <li> Choose $i=1$ and $j=2$, yielding the array $[1,1,0]$. </li><li> Choose $i=1$ and $j=3$, yielding the array $[0,1,1]$. </li><li> Choose $i=2$ and $j=3$, yielding the array $[0,0,2]$. </li></ul> At this point, $a_1=a_2=0$, completing the process.<p>In the second case, one possible sequence of operations is as follows. </p><ul> <li> Choose $i=4$ and $j=5$, yielding the array $[0,2,0,1,1]$. </li><li> Choose $i=2$ and $j=3$, yielding the array $[0,1,1,1,1]$. </li><li> Choose $i=2$ and $j=5$, yielding the array $[0,0,1,1,2]$. </li><li> Choose $i=3$ and $j=5$, yielding the array $[0,0,0,1,3]$. </li><li> Choose $i=4$ and $j=5$, yielding the array $[0,0,0,0,4]$. </li></ul><p>In the last case, the array already satisfies the condition.</p>
