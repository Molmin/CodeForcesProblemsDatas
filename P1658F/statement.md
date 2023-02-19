## Description

<div><p>The <span class="tex-font-style-it">cuteness</span> of a binary string is the number of $\texttt{1}$s divided by the length of the string. For example, the <span class="tex-font-style-it">cuteness</span> of $\texttt{01101}$ is $\frac{3}{5}$.</p><p>Juju has a binary string $s$ of length $n$. She wants to choose some non-intersecting subsegments of $s$ such that their concatenation has length $m$ and it has the same <span class="tex-font-style-it">cuteness</span> as the string $s$. </p><p>More specifically, she wants to find two arrays $l$ and $r$ of equal length $k$ such that $1 \leq l_1 \leq r_1 &lt; l_2 \leq r_2 &lt; \ldots &lt; l_k \leq r_k \leq n$, and also:</p><ul> <li> $\sum\limits_{i=1}^k (r_i - l_i + 1) = m$; </li><li> The <span class="tex-font-style-it">cuteness</span> of $s[l_1,r_1]+s[l_2,r_2]+\ldots+s[l_k,r_k]$ is equal to the <span class="tex-font-style-it">cuteness</span> of $s$, where $s[x, y]$ denotes the subsegment $s_x s_{x+1} \ldots s_y$, and $+$ denotes string concatenation. </li></ul><p>Juju does not like splitting the string into many parts, so she also wants to <span class="tex-font-style-bf">minimize</span> the value of $k$. Find the minimum value of $k$ such that there exist $l$ and $r$ that satisfy the constraints above or determine that it is impossible to find such $l$ and $r$ for any $k$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq m \leq n \leq 2 \cdot 10^5$).</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, if there is no valid pair of $l$ and $r$, print $-1$. </p><p>Otherwise, print $k + 1$ lines.</p><p>In the first line, print a number $k$ ($1 \leq k \leq m$) — the minimum number of subsegments required.</p><p>Then print $k$ lines, the $i$-th should contain $l_i$ and $r_i$ ($1 \leq l_i \leq r_i \leq n$) — the range of the $i$-th subsegment. Note that you should output the subsegments such that the inequality $l_1 \leq r_1 &lt; l_2 \leq r_2 &lt; \ldots &lt; l_k \leq r_k$ is true.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq m \leq n \leq 2 \cdot 10^5$).</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, if there is no valid pair of $l$ and $r$, print $-1$. </p><p>Otherwise, print $k + 1$ lines.</p><p>In the first line, print a number $k$ ($1 \leq k \leq m$) — the minimum number of subsegments required.</p><p>Then print $k$ lines, the $i$-th should contain $l_i$ and $r_i$ ($1 \leq l_i \leq r_i \leq n$) — the range of the $i$-th subsegment. Note that you should output the subsegments such that the inequality $l_1 \leq r_1 &lt; l_2 \leq r_2 &lt; \ldots &lt; l_k \leq r_k$ is true.</p>





```input1|2,3,6,7
4
4 2
0011
8 6
11000011
4 3
0101
5 5
11111
```




```output1
1
2 3
2
2 3
5 8
-1
1
1 5
```



## Note

<p>In the first example, the <span class="tex-font-style-it">cuteness</span> of $\texttt{0011}$ is the same as the <span class="tex-font-style-it">cuteness</span> of $\texttt{01}$.</p><p>In the second example, the <span class="tex-font-style-it">cuteness</span> of $\texttt{11000011}$ is $\frac{1}{2}$ and there is no subsegment of size $6$ with the same cuteness. So we must use $2$ disjoint subsegments $\texttt{10}$ and $\texttt{0011}$.</p><p>In the third example, there are $8$ ways to split the string such that $\sum\limits_{i=1}^k (r_i - l_i + 1) = 3$ but none of them has the same <span class="tex-font-style-it">cuteness</span> as $\texttt{0101}$.</p><p>In the last example, we don't have to split the string.</p>
