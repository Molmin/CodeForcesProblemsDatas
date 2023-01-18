## Description

<div><p>You are given a range of positive integers from $l$ to $r$.</p><p>Find such a pair of integers $(x, y)$ that $l \le x, y \le r$, $x \ne y$ and $x$ divides $y$.</p><p>If there are multiple answers, print any of them.</p><p>You are also asked to answer $T$ independent queries.</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 1000$) — the number of queries.</p><p>Each of the next $T$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le 998244353$) — inclusive borders of the range.</p><p>It is guaranteed that testset only includes queries, which have at least one suitable pair.</p></div><div class="output-specification"><p>Print $T$ lines, each line should contain the answer — two integers $x$ and $y$ such that $l \le x, y \le r$, $x \ne y$ and $x$ divides $y$. The answer in the $i$-th line should correspond to the $i$-th query from the input.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 1000$) — the number of queries.</p><p>Each of the next $T$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le 998244353$) — inclusive borders of the range.</p><p>It is guaranteed that testset only includes queries, which have at least one suitable pair.</p>

## Output

<p>Print $T$ lines, each line should contain the answer — two integers $x$ and $y$ such that $l \le x, y \le r$, $x \ne y$ and $x$ divides $y$. The answer in the $i$-th line should correspond to the $i$-th query from the input.</p><p>If there are multiple answers, print any of them.</p>





```input1
3
1 10
3 14
1 10
```




```output1
1 7
3 9
5 10
```


