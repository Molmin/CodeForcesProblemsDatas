## Description

<div><p>You are given a permutation $p$ of length $n$.</p><p>You can choose any subsequence, remove it from the permutation, and insert it at the beginning of the permutation keeping the same order.</p><p>For every $k$ from $0$ to $n$, find the minimal possible number of inversions in the permutation after you choose a subsequence of length exactly $k$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 50\,000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$)&nbsp;— the length of the permutation.</p><p>The second line of each test case contains the permutation $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$).</p><p>It is guaranteed that the total sum of $n$ doesn't exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output $n + 1$ integers. The $i$-th of them must be the answer for the subsequence length of $i - 1$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 50\,000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$)&nbsp;— the length of the permutation.</p><p>The second line of each test case contains the permutation $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$).</p><p>It is guaranteed that the total sum of $n$ doesn't exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case output $n + 1$ integers. The $i$-th of them must be the answer for the subsequence length of $i - 1$.</p>





```input1
3
1
1
4
4 2 1 3
5
5 1 3 2 4
```




```output1
0 0
4 2 2 1 4
5 4 2 2 1 5
```



## Note

<p>In the second test case: </p><ul> <li> For the length $0$: $[4, 2, 1, 3] \rightarrow [4, 2, 1, 3]$: $4$ inversions. </li><li> For the length $1$: $[4, 2, \mathbf{1}, 3] \rightarrow [1, 4, 2, 3]$: $2$ inversions. </li><li> For the length $2$: $[4, \mathbf{2}, \mathbf{1}, 3] \rightarrow [2, 1, 4, 3]$, or $[4, 2, \mathbf{1}, \textbf{3}] \rightarrow [1, 3, 4, 2]$: $2$ inversions. </li><li> For the length $3$: $[4, \mathbf{2}, \mathbf{1}, \mathbf{3}] \rightarrow [2, 1, 3, 4]$: $1$ inversion. </li><li> For the length $4$: $[\mathbf{4}, \mathbf{2}, \mathbf{1}, \mathbf{3}] \rightarrow [4, 2, 1, 3]$: $4$ inversions. </li></ul>
