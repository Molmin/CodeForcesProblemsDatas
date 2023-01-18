## Description

<div><p>For some array $c$, let's denote a <span class="tex-font-style-it">greedy subsequence</span> as a sequence of indices $p_1$, $p_2$, ..., $p_l$ such that $1 \le p_1 &lt; p_2 &lt; \dots &lt; p_l \le |c|$, and for each $i \in [1, l - 1]$, $p_{i + 1}$ is the minimum number such that $p_{i + 1} &gt; p_i$ and $c[p_{i + 1}] &gt; c[p_i]$.</p><p>You are given an array $a_1, a_2, \dots, a_n$. For each its subsegment of length $k$, calculate the length of its longest greedy subsequence.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 10^6$) — the length of array $a$ and the length of subsegments.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) — array $a$.</p></div><div class="output-specification"><p>Print $n - k + 1$ integers — the maximum lengths of greedy subsequences of each subsegment having length $k$. The first number should correspond to subsegment $a[1..k]$, the second — to subsegment $a[2..k + 1]$, and so on.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 10^6$) — the length of array $a$ and the length of subsegments.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) — array $a$.</p>

## Output

<p>Print $n - k + 1$ integers — the maximum lengths of greedy subsequences of each subsegment having length $k$. The first number should correspond to subsegment $a[1..k]$, the second — to subsegment $a[2..k + 1]$, and so on.</p>





```input1
6 4
1 5 2 5 3 6
```




```input2
7 6
4 5 2 5 3 6 6
```




```output1
2 2 3
```




```output2
3 3
```



## Note

<p>In the first example: </p><ul> <li> $[1, 5, 2, 5]$ — the longest greedy subsequences are $1, 2$ ($[c_1, c_2] = [1, 5]$) or $3, 4$ ($[c_3, c_4] = [2, 5]$). </li><li> $[5, 2, 5, 3]$ — the sequence is $2, 3$ ($[c_2, c_3] = [2, 5]$). </li><li> $[2, 5, 3, 6]$ — the sequence is $1, 2, 4$ ($[c_1, c_2, c_4] = [2, 5, 6]$). </li></ul><p>In the second example: </p><ul> <li> $[4, 5, 2, 5, 3, 6]$ — the longest greedy subsequences are $1, 2, 6$ ($[c_1, c_2, c_6] = [4, 5, 6]$) or $3, 4, 6$ ($[c_3, c_4, c_6] = [2, 5, 6]$). </li><li> $[5, 2, 5, 3, 6, 6]$ — the subsequence is $2, 3, 5$ ($[c_2, c_3, c_5] = [2, 5, 6]$). </li></ul>
