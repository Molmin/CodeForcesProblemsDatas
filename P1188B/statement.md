## Description

<div><p>You are given a <span class="tex-font-style-bf">prime</span> number $p$, $n$ integers $a_1, a_2, \ldots, a_n$, and an integer $k$. </p><p>Find the number of pairs of indexes $(i, j)$ ($1 \le i &lt; j \le n$) for which $(a_i + a_j)(a_i^2 + a_j^2) \equiv k \bmod p$.</p></div><div class="input-specification"><p>The first line contains integers $n, p, k$ ($2 \le n \le 3 \cdot 10^5$, $2 \le p \le 10^9$, $0 \le k \le p-1$). $p$ is guaranteed to be prime.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le p-1$). It is guaranteed that all elements are different.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— answer to the problem.</p></div>

## Input

<p>The first line contains integers $n, p, k$ ($2 \le n \le 3 \cdot 10^5$, $2 \le p \le 10^9$, $0 \le k \le p-1$). $p$ is guaranteed to be prime.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le p-1$). It is guaranteed that all elements are different.</p>

## Output

<p>Output a single integer&nbsp;— answer to the problem.</p>





```input1
3 3 0
0 1 2
```




```input2
6 7 2
1 2 3 4 5 6
```




```output1
1
```




```output2
3
```



## Note

<p>In the first example:</p><p>$(0+1)(0^2 + 1^2) = 1 \equiv 1 \bmod 3$.</p><p>$(0+2)(0^2 + 2^2) = 8 \equiv 2 \bmod 3$.</p><p>$(1+2)(1^2 + 2^2) = 15 \equiv 0 \bmod 3$.</p><p>So only $1$ pair satisfies the condition.</p><p>In the second example, there are $3$ such pairs: $(1, 5)$, $(2, 3)$, $(4, 6)$.</p>
