## Description

<div><p>You are given a set of $n$ ($n$ is always a power of $2$) elements containing all integers $0, 1, 2, \ldots, n-1$ exactly once.</p><p>Find $\frac{n}{2}$ pairs of elements such that:</p><ul> <li> Each element in the set is in exactly one pair. </li><li> The sum over all pairs of the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND</a> of its elements must be exactly equal to $k$. Formally, if $a_i$ and $b_i$ are the elements of the $i$-th pair, then the following must hold: $$\sum_{i=1}^{n/2}{a_i \&amp; b_i} = k,$$ where $\&amp;$ denotes the bitwise AND operation. </li></ul><p>If there are many solutions, print any of them, if there is no solution, print $-1$ instead.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 400$) — the number of test cases. Description of the test cases follows.</p><p>Each test case consists of a single line with two integers $n$ and $k$ ($4 \leq n \leq 2^{16}$, $n$ is a power of $2$, $0 \leq k \leq n-1$).</p><p>The sum of $n$ over all test cases does not exceed $2^{16}$. All test cases in each individual input will be pairwise <span class="tex-font-style-bf">different</span>.</p></div><div class="output-specification"><p>For each test case, if there is no solution, print a single line with the integer $-1$.</p><p>Otherwise, print $\frac{n}{2}$ lines, the $i$-th of them must contain $a_i$ and $b_i$, the elements in the $i$-th pair. </p><p>If there are many solutions, print any of them. Print the pairs and the elements in the pairs in any order.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 400$) — the number of test cases. Description of the test cases follows.</p><p>Each test case consists of a single line with two integers $n$ and $k$ ($4 \leq n \leq 2^{16}$, $n$ is a power of $2$, $0 \leq k \leq n-1$).</p><p>The sum of $n$ over all test cases does not exceed $2^{16}$. All test cases in each individual input will be pairwise <span class="tex-font-style-bf">different</span>.</p>

## Output

<p>For each test case, if there is no solution, print a single line with the integer $-1$.</p><p>Otherwise, print $\frac{n}{2}$ lines, the $i$-th of them must contain $a_i$ and $b_i$, the elements in the $i$-th pair. </p><p>If there are many solutions, print any of them. Print the pairs and the elements in the pairs in any order.</p>





```input1
4
4 0
4 1
4 2
4 3
```




```output1
0 3
1 2
0 2
1 3
0 1
2 3
-1
```



## Note

<p>In the first test, $(0\&amp;3)+(1\&amp;2) = 0$.</p><p>In the second test, $(0\&amp;2)+(1\&amp;3) = 1$.</p><p>In the third test, $(0\&amp;1)+(2\&amp;3) = 2$.</p><p>In the fourth test, there is no solution.</p>
