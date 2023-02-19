## Description

<div><p>You have an array $a$ consisting of $n$ distinct positive integers, numbered from $1$ to $n$. Define $p_k$ as $$p_k = \sum_{1 \le i, j \le k} a_i \bmod a_j,$$ where $x \bmod y$ denotes the remainder when $x$ is divided by $y$. You have to find and print $p_1, p_2, \ldots, p_n$. </p></div><div class="input-specification"><p>The first line contains $n$ — the length of the array ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ space-separated distinct integers $a_1, \ldots, a_n$ ($1 \le a_i \le 3 \cdot 10^5$, $a_i \neq a_j$ if $i \neq j$). </p></div><div class="output-specification"><p>Print $n$ integers $p_1, p_2, \ldots, p_n$. </p></div>

## Input

<p>The first line contains $n$ — the length of the array ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ space-separated distinct integers $a_1, \ldots, a_n$ ($1 \le a_i \le 3 \cdot 10^5$, $a_i \neq a_j$ if $i \neq j$). </p>

## Output

<p>Print $n$ integers $p_1, p_2, \ldots, p_n$. </p>





```input1
4
6 2 7 3
```




```input2
3
3 2 1
```




```output1
0 2 12 22
```




```output2
0 3 5
```


