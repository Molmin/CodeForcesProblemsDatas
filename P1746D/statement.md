## Description

<div><p>You are given a rooted tree consisting of $n$ vertices. The vertices are numbered from $1$ to $n$, and the root is the vertex $1$. You are also given a score array $s_1, s_2, \ldots, s_n$.</p><p>A multiset of $k$ simple paths is called valid if the following two conditions are both true. </p><ul> <li> Each path starts from $1$. </li><li> Let $c_i$ be the number of paths covering vertex $i$. For each pair of vertices $(u,v)$ ($2\le u,v\le n$) that have the same parent, $|c_u-c_v|\le 1$ holds. </li></ul> The <span class="tex-font-style-it">value</span> of the path multiset is defined as $\sum\limits_{i=1}^n c_i s_i$.<p>It can be shown that it is always possible to find at least one valid multiset. Find the maximum <span class="tex-font-style-it">value</span> among all valid multisets.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two space-separated integers $n$ ($2 \le n \le 2 \cdot 10^5$) and $k$ ($1 \le k \le 10^9$) — the size of the tree and the required number of paths.</p><p>The second line contains $n - 1$ space-separated integers $p_2,p_3,\ldots,p_n$ ($1\le p_i\le n$), where $p_i$ is the parent of the $i$-th vertex. It is guaranteed that this value describe a valid tree with root $1$.</p><p>The third line contains $n$ space-separated integers $s_1,s_2,\ldots,s_n$ ($0 \le s_i \le 10^4$) — the scores of the vertices.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10 ^ 5$.</p></div><div class="output-specification"><p>For each test case, print a single integer — the maximum <span class="tex-font-style-bf">value</span> of a path multiset.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two space-separated integers $n$ ($2 \le n \le 2 \cdot 10^5$) and $k$ ($1 \le k \le 10^9$) — the size of the tree and the required number of paths.</p><p>The second line contains $n - 1$ space-separated integers $p_2,p_3,\ldots,p_n$ ($1\le p_i\le n$), where $p_i$ is the parent of the $i$-th vertex. It is guaranteed that this value describe a valid tree with root $1$.</p><p>The third line contains $n$ space-separated integers $s_1,s_2,\ldots,s_n$ ($0 \le s_i \le 10^4$) — the scores of the vertices.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10 ^ 5$.</p>

## Output

<p>For each test case, print a single integer — the maximum <span class="tex-font-style-bf">value</span> of a path multiset.</p>





```input1|2,3,4
2
5 4
1 2 1 3
6 2 1 5 7
5 3
1 2 1 3
6 6 1 4 10
```




```output1
54
56
```



## Note

<p>In the first test case, one of optimal solutions is four paths $1 \to 2 \to 3 \to 5$, $1 \to 2 \to 3 \to 5$, $1 \to 4$, $1 \to 4$, here $c=[4,2,2,2,2]$. The value equals to $4\cdot 6+ 2\cdot 2+2\cdot 1+2\cdot 5+2\cdot 7=54$.</p><p>In the second test case, one of optimal solution is three paths $1 \to 2 \to 3 \to 5$, $1 \to 2 \to 3 \to 5$, $1 \to 4$, here $c=[3,2,2,1,2]$. The value equals to $3\cdot 6+ 2\cdot 6+2\cdot 1+1\cdot 4+2\cdot 10=56$.</p>
