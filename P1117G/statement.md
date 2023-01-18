## Description

<div><p>You are given a permutation $p_1, p_2, \dots, p_n$. You should answer $q$ queries. Each query is a pair $(l_i, r_i)$, and you should calculate $f(l_i, r_i)$.</p><p>Let's denote $m_{l, r}$ as the position of the maximum in subsegment $p_l, p_{l+1}, \dots, p_r$.</p><p>Then $f(l, r) = (r - l + 1) + f(l, m_{l,r} - 1) + f(m_{l,r} + 1, r)$ if $l \le r$ or $0$ otherwise.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n \le 10^6$, $1 \le q \le 10^6$) — the size of the permutation $p$ and the number of queries.</p><p>The second line contains $n$ pairwise distinct integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$, $p_i \neq p_j$ for $i \neq j$) — permutation $p$.</p><p>The third line contains $q$ integers $l_1, l_2, \dots, l_q$ — the first parts of the queries.</p><p>The fourth line contains $q$ integers $r_1, r_2, \dots, r_q$ — the second parts of the queries.</p><p>It's guaranteed that $1 \le l_i \le r_i \le n$ for all queries.</p></div><div class="output-specification"><p>Print $q$ integers — the values $f(l_i, r_i)$ for the corresponding queries.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n \le 10^6$, $1 \le q \le 10^6$) — the size of the permutation $p$ and the number of queries.</p><p>The second line contains $n$ pairwise distinct integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$, $p_i \neq p_j$ for $i \neq j$) — permutation $p$.</p><p>The third line contains $q$ integers $l_1, l_2, \dots, l_q$ — the first parts of the queries.</p><p>The fourth line contains $q$ integers $r_1, r_2, \dots, r_q$ — the second parts of the queries.</p><p>It's guaranteed that $1 \le l_i \le r_i \le n$ for all queries.</p>

## Output

<p>Print $q$ integers — the values $f(l_i, r_i)$ for the corresponding queries.</p>





```input1
4 5
3 1 4 2
2 1 1 2 1
2 3 4 4 1
```




```output1
1 6 8 5 1
```



## Note

<p>Description of the queries: </p><ol> <li> $f(2, 2) = (2 - 2 + 1) + f(2, 1) + f(3, 2) = 1 + 0 + 0 = 1$; </li><li> $f(1, 3) = (3 - 1 + 1) + f(1, 2) + f(4, 3) = 3 + (2 - 1 + 1) + f(1, 0) + f(2, 2) = 3 + 2 + (2 - 2 + 1) = 6$; </li><li> $f(1, 4) = (4 - 1 + 1) + f(1, 2) + f(4, 4) = 4 + 3 + 1 = 8$; </li><li> $f(2, 4) = (4 - 2 + 1) + f(2, 2) + f(4, 4) = 3 + 1 + 1 = 5$; </li><li> $f(1, 1) = (1 - 1 + 1) + 0 + 0 = 1$. </li></ol>
