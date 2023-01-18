## Description

<div><p>Let $\text{LCP}(s, t)$ be the length of the longest common prefix of strings $s$ and $t$. Also let $s[x \dots y]$ be the substring of $s$ from index $x$ to index $y$ (inclusive). For example, if $s = $ "<span class="tex-font-style-tt">abcde</span>", then $s[1 \dots 3] =$ "<span class="tex-font-style-tt">abc</span>", $s[2 \dots 5] =$ "<span class="tex-font-style-tt">bcde</span>".</p><p>You are given a string $s$ of length $n$ and $q$ queries. Each query is a pair of integer sets $a_1, a_2, \dots, a_k$ and $b_1, b_2, \dots, b_l$. Calculate $\sum\limits_{i = 1}^{i = k} \sum\limits_{j = 1}^{j = l}{\text{LCP}(s[a_i \dots n], s[b_j \dots n])}$ for each query.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$) — the length of string $s$ and the number of queries, respectively.</p><p>The second line contains a string $s$ consisting of lowercase Latin letters ($|s| = n$).</p><p>Next $3q$ lines contains descriptions of queries — three lines per query. The first line of each query contains two integers $k_i$ and $l_i$ ($1 \le k_i, l_i \le n$) — sizes of sets $a$ and $b$ respectively.</p><p>The second line of each query contains $k_i$ integers $a_1, a_2, \dots a_{k_i}$ ($1 \le a_1 &lt; a_2 &lt; \dots &lt; a_{k_i} \le n$) — set $a$.</p><p>The third line of each query contains $l_i$ integers $b_1, b_2, \dots b_{l_i}$ ($1 \le b_1 &lt; b_2 &lt; \dots &lt; b_{l_i} \le n$) — set $b$.</p><p>It is guaranteed that $\sum\limits_{i = 1}^{i = q}{k_i} \le 2 \cdot 10^5$ and $\sum\limits_{i = 1}^{i = q}{l_i} \le 2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $q$ integers — answers for the queries in the same order queries are given in the input.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$) — the length of string $s$ and the number of queries, respectively.</p><p>The second line contains a string $s$ consisting of lowercase Latin letters ($|s| = n$).</p><p>Next $3q$ lines contains descriptions of queries — three lines per query. The first line of each query contains two integers $k_i$ and $l_i$ ($1 \le k_i, l_i \le n$) — sizes of sets $a$ and $b$ respectively.</p><p>The second line of each query contains $k_i$ integers $a_1, a_2, \dots a_{k_i}$ ($1 \le a_1 &lt; a_2 &lt; \dots &lt; a_{k_i} \le n$) — set $a$.</p><p>The third line of each query contains $l_i$ integers $b_1, b_2, \dots b_{l_i}$ ($1 \le b_1 &lt; b_2 &lt; \dots &lt; b_{l_i} \le n$) — set $b$.</p><p>It is guaranteed that $\sum\limits_{i = 1}^{i = q}{k_i} \le 2 \cdot 10^5$ and $\sum\limits_{i = 1}^{i = q}{l_i} \le 2 \cdot 10^5$.</p>

## Output

<p>Print $q$ integers — answers for the queries in the same order queries are given in the input.</p>





```input1
7 4
abacaba
2 2
1 2
1 2
3 1
1 2 3
7
1 7
1
1 2 3 4 5 6 7
2 2
1 5
1 5

```




```output1
13
2
12
16

```



## Note

<p>Description of queries: </p><ol> <li> In the first query $s[1 \dots 7] = \text{abacaba}$ and $s[2 \dots 7] = \text{bacaba}$ are considered. The answer for the query is $\text{LCP}(\text{abacaba}, \text{abacaba}) + \text{LCP}(\text{abacaba}, \text{bacaba}) + \text{LCP}(\text{bacaba}, \text{abacaba}) + \text{LCP}(\text{bacaba}, \text{bacaba}) = 7 + 0 + 0 + 6 = 13$.</li><li> In the second query $s[1 \dots 7] = \text{abacaba}$, $s[2 \dots 7] = \text{bacaba}$, $s[3 \dots 7] = \text{acaba}$ and $s[7 \dots 7] = \text{a}$ are considered. The answer for the query is $\text{LCP}(\text{abacaba}, \text{a}) + \text{LCP}(\text{bacaba}, \text{a}) + \text{LCP}(\text{acaba}, \text{a}) = 1 + 0 + 1 = 2$.</li><li> In the third query $s[1 \dots 7] = \text{abacaba}$ are compared with all suffixes. The answer is the sum of non-zero values: $\text{LCP}(\text{abacaba}, \text{abacaba}) + \text{LCP}(\text{abacaba}, \text{acaba}) + \text{LCP}(\text{abacaba}, \text{aba}) + \text{LCP}(\text{abacaba}, \text{a}) = 7 + 1 + 3 + 1 = 12$.</li><li> In the fourth query $s[1 \dots 7] = \text{abacaba}$ and $s[5 \dots 7] = \text{aba}$ are considered. The answer for the query is $\text{LCP}(\text{abacaba}, \text{abacaba}) + \text{LCP}(\text{abacaba}, \text{aba}) + \text{LCP}(\text{aba}, \text{abacaba}) + \text{LCP}(\text{aba}, \text{aba}) = 7 + 3 + 3 + 3 = 16$. </li></ol>
