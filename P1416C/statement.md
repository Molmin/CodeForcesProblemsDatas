## Description

<div><p>You are given an array $a$ consisting of $n$ non-negative integers. You have to choose a non-negative integer $x$ and form a new array $b$ of size $n$ according to the following rule: for all $i$ from $1$ to $n$, $b_i = a_i \oplus x$ ($\oplus$ denotes the operation <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a>).</p><p>An inversion in the $b$ array is a pair of integers $i$ and $j$ such that $1 \le i &lt; j \le n$ and $b_i &gt; b_j$.</p><p>You should choose $x$ in such a way that the number of inversions in $b$ is minimized. If there are several options for $x$ — output the smallest one.</p></div><div class="input-specification"><p>First line contains a single integer $n$ ($1 \le n \le 3 \cdot 10^5$) — the number of elements in $a$.</p><p>Second line contains $n$ space-separated integers $a_1$, $a_2$, ..., $a_n$ ($0 \le a_i \le 10^9$), where $a_i$ is the $i$-th element of $a$.</p></div><div class="output-specification"><p>Output two integers: the minimum possible number of inversions in $b$, and the minimum possible value of $x$, which achieves those number of inversions.</p></div>

## Input

<p>First line contains a single integer $n$ ($1 \le n \le 3 \cdot 10^5$) — the number of elements in $a$.</p><p>Second line contains $n$ space-separated integers $a_1$, $a_2$, ..., $a_n$ ($0 \le a_i \le 10^9$), where $a_i$ is the $i$-th element of $a$.</p>

## Output

<p>Output two integers: the minimum possible number of inversions in $b$, and the minimum possible value of $x$, which achieves those number of inversions.</p>





```input1
4
0 1 3 2
```




```input2
9
10 7 9 10 7 5 5 3 5
```




```input3
3
8 10 3
```




```output1
1 0
```




```output2
4 14
```




```output3
0 8
```



## Note

<p>In the first sample it is optimal to leave the array as it is by choosing $x = 0$.</p><p>In the second sample the selection of $x = 14$ results in $b$: $[4, 9, 7, 4, 9, 11, 11, 13, 11]$. It has $4$ inversions:</p><ul> <li> $i = 2$, $j = 3$; </li><li> $i = 2$, $j = 4$; </li><li> $i = 3$, $j = 4$; </li><li> $i = 8$, $j = 9$. </li></ul><p>In the third sample the selection of $x = 8$ results in $b$: $[0, 2, 11]$. It has no inversions.</p>
