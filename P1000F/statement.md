## Description

<div><p>You are given an array $a$ consisting of $n$ integers, and $q$ queries to it. $i$-th query is denoted by two integers $l_i$ and $r_i$. For each query, you have to find <span class="tex-font-style-bf">any</span> integer that occurs <span class="tex-font-style-bf">exactly once</span> in the subarray of $a$ from index $l_i$ to index $r_i$ (a subarray is a contiguous subsegment of an array). For example, if $a = [1, 1, 2, 3, 2, 4]$, then for query $(l_i = 2, r_i = 6)$ the subarray we are interested in is $[1, 2, 3, 2, 4]$, and possible answers are $1$, $3$ and $4$; for query $(l_i = 1, r_i = 2)$ the subarray we are interested in is $[1, 1]$, and there is no such element that occurs exactly once.</p><p>Can you answer all of the queries?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 5 \cdot 10^5$).</p><p>The third line contains one integer $q$ ($1 \le q \le 5 \cdot 10^5$).</p><p>Then $q$ lines follow, $i$-th line containing two integers $l_i$ and $r_i$ representing $i$-th query ($1 \le l_i \le r_i \le n$).</p></div><div class="output-specification"><p>Answer the queries as follows:</p><p>If there is no integer such that it occurs in the subarray from index $l_i$ to index $r_i$ exactly once, print $0$. Otherwise print any such integer.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 5 \cdot 10^5$).</p><p>The third line contains one integer $q$ ($1 \le q \le 5 \cdot 10^5$).</p><p>Then $q$ lines follow, $i$-th line containing two integers $l_i$ and $r_i$ representing $i$-th query ($1 \le l_i \le r_i \le n$).</p>

## Output

<p>Answer the queries as follows:</p><p>If there is no integer such that it occurs in the subarray from index $l_i$ to index $r_i$ exactly once, print $0$. Otherwise print any such integer.</p>





```input1
6
1 1 2 3 2 4
2
2 6
1 2

```




```output1
4
0

```


