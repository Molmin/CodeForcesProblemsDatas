## Description

<div><p>Denote a cyclic sequence of size $n$ as an array $s$ such that $s_n$ is adjacent to $s_1$. The segment $s[r, l]$ where $l &lt; r$ is the concatenation of $s[r, n]$ and $s[1, l]$.</p><p>You are given an array $a$ consisting of $n$ integers. Define $b$ as the cyclic sequence obtained from concatenating $m$ copies of $a$. Note that $b$ has size $n \cdot m$.</p><p>You are given an integer $k$ where $k = 1$ or $k$ is a prime number. Find the number of different segments in $b$ where the sum of elements in the segment is divisible by $k$.</p><p><span class="tex-font-style-bf">Two segments are considered different if the set of indices of the segments are different</span>. For example, when $n = 3$ and $m = 2$, the set of indices for segment $s[2, 5]$ is $\{2, 3, 4, 5\}$, and for segment $s[5, 2]$ is $\{5, 6, 1, 2\}$. In particular, the segments $s[1, 6], s[2,1], \ldots, s[6, 5]$ are considered as the same segment.</p><p>Output the answer modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, and $k$ ($1 \leq n, m, k \leq 2 \cdot 10^5$, $k = 1$ or $k$ is a prime number).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 2 \cdot 10^5$).</p></div><div class="output-specification"><p>Output an integer denoting the number of different segments in $b$ where the sum of elements in the segment is divisible by $k$, modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, and $k$ ($1 \leq n, m, k \leq 2 \cdot 10^5$, $k = 1$ or $k$ is a prime number).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 2 \cdot 10^5$).</p>

## Output

<p>Output an integer denoting the number of different segments in $b$ where the sum of elements in the segment is divisible by $k$, modulo $10^9 + 7$.</p>





```input1
5 1 5
1 2 3 4 3
```




```input2
5 1 5
1 2 3 4 5
```




```input3
5 4 5
1 2 3 4 5
```




```output1
4
```




```output2
5
```




```output3
125
```



## Note

<p>In the first example, all valid segments are $[1,4]$, $[2, 3]$, $[3, 5]$, and $[4, 2]$.</p><p>In the second example, one of the valid segments is $[1, 5]$.</p>
