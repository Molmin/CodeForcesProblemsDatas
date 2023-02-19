## Description

<div><p>You are given a permutation $p$ of integers from $0$ to $n-1$ (each of them occurs exactly once). Initially, the permutation is <span class="tex-font-style-bf">not sorted</span> (that is, $p_i&gt;p_{i+1}$ for at least one $1 \le i \le n - 1$). </p><p>The permutation is called $X$-sortable for some non-negative integer $X$ if it is possible to sort the permutation by performing the operation below some finite number of times: </p><ul> <li> Choose two indices $i$ and $j$ $(1 \le i \lt j \le n)$ such that $p_i \&amp; p_j = X$. </li><li> Swap $p_i$ and $p_j$. </li></ul><p>Here $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>.</p><p>Find the <span class="tex-font-style-bf">maximum</span> value of $X$ such that $p$ is $X$-sortable. It can be shown that there always exists some value of $X$ such that $p$ is $X$-sortable.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ $(1 \le t \le 10^4)$ &nbsp;— the number of test cases. Description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2 \le n \le 2 \cdot 10^5)$ &nbsp;— the length of the permutation.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, ..., p_n$ ($0 \le p_i \le n-1$, all $p_i$ are distinct) &nbsp;— the elements of $p$. It is guaranteed that $p$ is not sorted.</p><p>It is guaranteed that the sum of $n$ over all cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output a single integer — the maximum value of $X$ such that $p$ is $X$-sortable.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ $(1 \le t \le 10^4)$ &nbsp;— the number of test cases. Description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2 \le n \le 2 \cdot 10^5)$ &nbsp;— the length of the permutation.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, ..., p_n$ ($0 \le p_i \le n-1$, all $p_i$ are distinct) &nbsp;— the elements of $p$. It is guaranteed that $p$ is not sorted.</p><p>It is guaranteed that the sum of $n$ over all cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output a single integer — the maximum value of $X$ such that $p$ is $X$-sortable.</p>





```input1
4
4
0 1 3 2
2
1 0
7
0 1 2 3 5 6 4
5
0 3 2 1 4
```




```output1
2
0
4
1
```



## Note

<p>In the first test case, the only $X$ for which the permutation is $X$-sortable are $X = 0$ and $X = 2$, maximum of which is $2$.</p><p>Sorting using $X = 0$: </p><ul> <li> Swap $p_1$ and $p_4$, $p = [2, 1, 3, 0]$. </li><li> Swap $p_3$ and $p_4$, $p = [2, 1, 0, 3]$. </li><li> Swap $p_1$ and $p_3$, $p = [0, 1, 2, 3]$. </li></ul><p>Sorting using $X = 2$: </p><ul> <li> Swap $p_3$ and $p_4$, $p = [0, 1, 2, 3]$. </li></ul><p>In the second test case, we must swap $p_1$ and $p_2$ which is possible only with $X = 0$.</p>
