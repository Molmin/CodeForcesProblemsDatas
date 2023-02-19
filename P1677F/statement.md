## Description

<div><p>Tokitsukaze has a sequence with length of $n$. She likes gems very much. There are $n$ kinds of gems. The gems of the $i$-th kind are on the $i$-th position, and there are $a_i$ gems of the same kind on that position. Define $G(l,r)$ as the multiset containing all gems on the segment $[l,r]$ (inclusive).</p><p>A multiset of gems can be represented as $S=[s_1,s_2,\ldots,s_n]$, which is a non-negative integer sequence of length $n$ and means that $S$ contains $s_i$ gems of the $i$-th kind in the multiset. A multiset $T=[t_1,t_2,\ldots,t_n]$ is a multisubset of $S=[s_1,s_2,\ldots,s_n]$ if and only if $t_i\le s_i$ for any $i$ satisfying $1\le i\le n$.</p><p>Now, given two positive integers $k$ and $p$, you need to calculate the result of</p><p>$$\sum_{l=1}^n \sum_{r=l}^n\sum\limits_{[t_1,t_2,\cdots,t_n] \subseteq G(l,r)}\left(\left(\sum_{i=1}^n p^{t_i}t_i^k\right)\left(\sum_{i=1}^n[t_i&gt;0]\right)\right),$$</p><p>where $[t_i&gt;0]=1$ if $t_i&gt;0$ and $[t_i&gt;0]=0$ if $t_i=0$.</p><p>Since the answer can be quite large, print it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $k$ and $p$ ($1\le n \le 10^5$; $1\le k\le 10^5$; $2\le p\le 998\,244\,351$)&nbsp;— the length of the sequence, the numbers $k$ and $p$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1\le a_i\le 998\,244\,351$)&nbsp;— the number of gems on the $i$-th position.</p></div><div class="output-specification"><p>Print a single integers&nbsp;— the result modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains three integers $n$, $k$ and $p$ ($1\le n \le 10^5$; $1\le k\le 10^5$; $2\le p\le 998\,244\,351$)&nbsp;— the length of the sequence, the numbers $k$ and $p$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1\le a_i\le 998\,244\,351$)&nbsp;— the number of gems on the $i$-th position.</p>

## Output

<p>Print a single integers&nbsp;— the result modulo $998\,244\,353$.</p>





```input1
5 2 2
1 1 1 2 2
```




```input2
6 2 2
2 2 2 2 2 3
```




```output1
6428
```




```output2
338940
```


