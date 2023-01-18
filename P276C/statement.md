## Description

<div><p>The little girl loves the problems on array queries very much.</p><p>One day she came across a rather well-known problem: you've got an array of $n$ elements (the elements of the array are indexed starting from 1); also, there are $q$ queries, each one is defined by a pair of integers $l_i$, $r_i$ $(1 \le l_i \le r_i \le n)$. You need to find for each query the sum of elements of the array with indexes from $l_i$ to $r_i$, inclusive.</p><p>The little girl found the problem rather boring. She decided to reorder the array elements before replying to the queries in a way that makes the sum of query replies maximum possible. Your task is to find the value of this maximum sum.</p></div><div class="input-specification"><p>The first line contains two space-separated integers $n$ ($1 \le n \le 2\cdot10^5$) and $q$ ($1 \le q \le 2\cdot10^5$) — the number of elements in the array and the number of queries, correspondingly.</p><p>The next line contains $n$ space-separated integers $a_i$ ($1 \le a_i \le 2\cdot10^5$) — the array elements.</p><p>Each of the following $q$ lines contains two space-separated integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$) — the $i$-th query.</p></div><div class="output-specification"><p>In a single line print, a single integer — the maximum sum of query replies after the array elements are reordered.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two space-separated integers $n$ ($1 \le n \le 2\cdot10^5$) and $q$ ($1 \le q \le 2\cdot10^5$) — the number of elements in the array and the number of queries, correspondingly.</p><p>The next line contains $n$ space-separated integers $a_i$ ($1 \le a_i \le 2\cdot10^5$) — the array elements.</p><p>Each of the following $q$ lines contains two space-separated integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$) — the $i$-th query.</p>

## Output

<p>In a single line print, a single integer — the maximum sum of query replies after the array elements are reordered.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3 3
5 3 2
1 2
2 3
1 3

```




```input2
5 3
5 2 4 1 3
1 5
2 3
2 3

```




```output1
25

```




```output2
33

```


