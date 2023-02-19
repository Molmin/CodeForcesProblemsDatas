## Description

<div><p>You are given an integer array $a$ of size $n$.</p><p>You have to perform $m$ queries. Each query has one of two types: </p><ul> <li> "$1$ $l$ $r$ $k$" — calculate the minimum value $dif$ such that there are exist $k$ <span class="tex-font-style-bf">distinct</span> integers $x_1, x_2, \dots, x_k$ such that $cnt_i &gt; 0$ (for every $i \in [1, k]$) and $|cnt_i - cnt_j| \le dif$ (for every $i \in [1, k], j \in [1, k]$), where $cnt_i$ is the number of occurrences of $x_i$ in the subarray $a[l..r]$. If it is impossible to choose $k$ integers, report it; </li><li> "$2$ $p$ $x$" — assign $a_{p} := x$. </li></ul></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 10^5$) — the size of the array $a$ and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$).</p><p>Next $m$ lines contain queries (one per line). Each query has one of two types: </p><ul> <li> "$1$ $l$ $r$ $k$" ($1 \le l \le r \le n; 1 \le k \le 10^5$) </li><li> "$2$ $p$ $x$" ($1 \le p \le n; 1 \le x \le 10^5$). </li></ul><p>It's guaranteed that there is at least one query of the first type.</p></div><div class="output-specification"><p>For each query of the first type, print the minimum value of $dif$ that satisfies all required conditions, or $-1$ if it is impossible to choose $k$ distinct integers.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 10^5$) — the size of the array $a$ and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$).</p><p>Next $m$ lines contain queries (one per line). Each query has one of two types: </p><ul> <li> "$1$ $l$ $r$ $k$" ($1 \le l \le r \le n; 1 \le k \le 10^5$) </li><li> "$2$ $p$ $x$" ($1 \le p \le n; 1 \le x \le 10^5$). </li></ul><p>It's guaranteed that there is at least one query of the first type.</p>

## Output

<p>For each query of the first type, print the minimum value of $dif$ that satisfies all required conditions, or $-1$ if it is impossible to choose $k$ distinct integers.</p>





```input1
12 11
2 1 1 2 1 1 3 2 1 1 3 3
1 2 10 3
1 2 11 3
2 7 2
1 3 9 2
1 1 12 1
1 1 12 4
2 12 4
1 1 12 4
2 1 5
1 3 12 2
1 1 4 3
```




```output1
5
4
1
0
-1
5
0
1
```


