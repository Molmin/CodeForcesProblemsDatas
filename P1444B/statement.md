## Description

<div><p>You are given an array $a$ of length $2n$. Consider a partition of array $a$ into two subsequences $p$ and $q$ of length $n$ each (each element of array $a$ should be in exactly one subsequence: either in $p$ or in $q$).</p><p>Let's sort $p$ in non-decreasing order, and $q$ in non-increasing order, we can denote the sorted versions by $x$ and $y$, respectively. Then the <span class="tex-font-style-it">cost</span> of a partition is defined as $f(p, q) = \sum_{i = 1}^n |x_i - y_i|$.</p><p>Find the sum of $f(p, q)$ over all correct partitions of array $a$. Since the answer might be too big, print its remainder modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 150\,000$).</p><p>The second line contains $2n$ integers $a_1, a_2, \ldots, a_{2n}$ ($1 \leq a_i \leq 10^9$)&nbsp;— elements of array $a$.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the answer to the problem, modulo $998244353$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 150\,000$).</p><p>The second line contains $2n$ integers $a_1, a_2, \ldots, a_{2n}$ ($1 \leq a_i \leq 10^9$)&nbsp;— elements of array $a$.</p>

## Output

<p>Print one integer&nbsp;— the answer to the problem, modulo $998244353$.</p>





```input1
1
1 4
```




```input2
2
2 1 2 1
```




```input3
3
2 2 2 2 2 2
```




```input4
5
13 8 35 94 9284 34 54 69 123 846
```




```output1
6
```




```output2
12
```




```output3
0
```




```output4
2588544
```



## Note

<p>Two partitions of an array are considered different if the sets of indices of elements included in the subsequence $p$ are different.</p><p>In the first example, there are two correct partitions of the array $a$:</p><ol> <li> $p = [1]$, $q = [4]$, then $x = [1]$, $y = [4]$, $f(p, q) = |1 - 4| = 3$; </li><li> $p = [4]$, $q = [1]$, then $x = [4]$, $y = [1]$, $f(p, q) = |4 - 1| = 3$. </li></ol><p>In the second example, there are six valid partitions of the array $a$: </p><ol> <li> $p = [2, 1]$, $q = [2, 1]$ (elements with indices $1$ and $2$ in the original array are selected in the subsequence $p$); </li><li> $p = [2, 2]$, $q = [1, 1]$; </li><li> $p = [2, 1]$, $q = [1, 2]$ (elements with indices $1$ and $4$ are selected in the subsequence $p$); </li><li> $p = [1, 2]$, $q = [2, 1]$; </li><li> $p = [1, 1]$, $q = [2, 2]$; </li><li> $p = [2, 1]$, $q = [2, 1]$ (elements with indices $3$ and $4$ are selected in the subsequence $p$). </li></ol>
