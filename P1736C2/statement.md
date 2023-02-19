## Description

<div><p><span class="tex-font-style-it">This is the hard version of this problem. In this version, we have queries. Note that we do not have multiple test cases in this version. You can make hacks only if both versions of the problem are solved.</span></p><p>An array $b$ of length $m$ is <span class="tex-font-style-it">good</span> if for all $i$ the $i$-th element is greater than or equal to $i$. In other words, $b$ is <span class="tex-font-style-it">good</span> if and only if $b_i \geq i$ for all $i$ ($1 \leq i \leq m$).</p><p>You are given an array $a$ consisting of $n$ positive integers, and you are asked $q$ queries. </p><p>In each query, you are given two integers $p$ and $x$ ($1 \leq p,x \leq n$). You have to do $a_p := x$ (assign $x$ to $a_p$). In the updated array, find the number of pairs of indices $(l, r)$, where $1 \le l \le r \le n$, such that the array $[a_l, a_{l+1}, \ldots, a_r]$ is <span class="tex-font-style-it">good</span>.</p><p>Note that all queries are <span class="tex-font-style-bf">independent</span>, which means after each query, the initial array $a$ is restored. </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$).</p><p>The third line contains an integer $q$ ($1 \leq q \leq 2 \cdot 10^5$) — the number of queries.</p><p>Each of the next $q$ lines contains two integers $p_j$ and $x_j$ ($1 \leq p_j, x_j \leq n$) – the description of the $j$-th query.</p></div><div class="output-specification"><p>For each query, print the number of suitable pairs of indices after making the change. </p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$).</p><p>The third line contains an integer $q$ ($1 \leq q \leq 2 \cdot 10^5$) — the number of queries.</p><p>Each of the next $q$ lines contains two integers $p_j$ and $x_j$ ($1 \leq p_j, x_j \leq n$) – the description of the $j$-th query.</p>

## Output

<p>For each query, print the number of suitable pairs of indices after making the change. </p>





```input1
4
2 4 1 4
3
2 4
3 3
2 1
```




```input2
5
1 1 3 2 1
3
1 3
2 5
4 5
```




```output1
6
10
5
```




```output2
7
9
8
```



## Note

<p>Here are notes for first example.</p><p>In first query, after update $a=[2,4,1,4]$. Now $(1,1)$, $(2,2)$, $(3,3)$, $(4,4)$, $(1,2)$, and $(3,4)$ are suitable pairs.</p><p>In second query, after update $a=[2,4,3,4]$. Now all subarrays of $a$ are <span class="tex-font-style-tt">good</span>.</p><p>In third query, after update $a=[2,1,1,4]$. Now $(1,1)$, $(2,2)$, $(3,3)$, $(4,4)$, and $(3,4)$ are suitable.</p>
