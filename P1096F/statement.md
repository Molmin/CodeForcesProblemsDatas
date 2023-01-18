## Description

<div><p>A permutation of size $n$ is an array of size $n$ such that each integer from $1$ to $n$ occurs exactly once in this array. An inversion in a permutation $p$ is a pair of indices $(i, j)$ such that $i &gt; j$ and $a_i &lt; a_j$. For example, a permutation $[4, 1, 3, 2]$ contains $4$ inversions: $(2, 1)$, $(3, 1)$, $(4, 1)$, $(4, 3)$.</p><p>You are given a permutation $p$ of size $n$. However, the numbers on some positions are replaced by $-1$. Let the valid permutation be such a replacement of $-1$ in this sequence back to numbers from $1$ to $n$ in such a way that the resulting sequence is a permutation of size $n$.</p><p>The given sequence was turned into a valid permutation randomly with the equal probability of getting each valid permutation.</p><p>Calculate the expected total number of inversions in the resulting valid permutation.</p><p>It can be shown that it is in the form of $\frac{P}{Q}$ where $P$ and $Q$ are non-negative integers and $Q \ne 0$. Report the value of $P \cdot Q^{-1} \pmod {998244353}$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of the sequence.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($-1 \le p_i \le n$, $p_i \ne 0$) — the initial sequence.</p><p>It is guaranteed that all elements not equal to $-1$ are pairwise distinct.</p></div><div class="output-specification"><p>Print a single integer — the expected total number of inversions in the resulting valid permutation.</p><p>It can be shown that it is in the form of $\frac{P}{Q}$ where $P$ and $Q$ are non-negative integers and $Q \ne 0$. Report the value of $P \cdot Q^{-1} \pmod {998244353}$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of the sequence.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($-1 \le p_i \le n$, $p_i \ne 0$) — the initial sequence.</p><p>It is guaranteed that all elements not equal to $-1$ are pairwise distinct.</p>

## Output

<p>Print a single integer — the expected total number of inversions in the resulting valid permutation.</p><p>It can be shown that it is in the form of $\frac{P}{Q}$ where $P$ and $Q$ are non-negative integers and $Q \ne 0$. Report the value of $P \cdot Q^{-1} \pmod {998244353}$.</p>





```input1
3
3 -1 -1
```




```input2
2
1 2
```




```input3
2
-1 -1
```




```output1
499122179
```




```output2
0
```




```output3
499122177
```



## Note

<p>In the first example two resulting valid permutations are possible:</p><ul> <li> $[3, 1, 2]$ — $2$ inversions; </li><li> $[3, 2, 1]$ — $3$ inversions. </li></ul><p>The expected value is $\frac{2 \cdot 1 + 3 \cdot 1}{2} = 2.5$.</p><p>In the second example no $-1$ are present, thus the only valid permutation is possible — the given one. It has $0$ inversions.</p><p>In the third example there are two resulting valid permutations — one with $0$ inversions and one with $1$ inversion.</p>
