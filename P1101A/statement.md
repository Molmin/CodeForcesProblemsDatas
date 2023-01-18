## Description

<div><p>You are given $q$ queries in the following form:</p><p><span class="tex-font-style-it">Given three integers $l_i$, $r_i$ and $d_i$, find minimum <span class="tex-font-style-bf">positive</span> integer $x_i$ such that it is divisible by $d_i$ and it does not belong to the segment $[l_i, r_i]$</span>.</p><p>Can you answer all the queries?</p><p><span class="tex-font-style-it">Recall that a number $x$ belongs to segment $[l, r]$ if $l \le x \le r$</span>.</p></div><div class="input-specification"><p>The first line contains one integer $q$ ($1 \le q \le 500$) — the number of queries.</p><p>Then $q$ lines follow, each containing a query given in the format $l_i$ $r_i$ $d_i$ ($1 \le l_i \le r_i \le 10^9$, $1 \le d_i \le 10^9$). $l_i$, $r_i$ and $d_i$ are integers.</p></div><div class="output-specification"><p>For each query print one integer: the answer to this query.</p></div>

## Input

<p>The first line contains one integer $q$ ($1 \le q \le 500$) — the number of queries.</p><p>Then $q$ lines follow, each containing a query given in the format $l_i$ $r_i$ $d_i$ ($1 \le l_i \le r_i \le 10^9$, $1 \le d_i \le 10^9$). $l_i$, $r_i$ and $d_i$ are integers.</p>

## Output

<p>For each query print one integer: the answer to this query.</p>





```input1
5
2 4 2
5 10 4
3 10 1
1 2 3
4 6 5
```




```output1
6
4
1
3
10
```


