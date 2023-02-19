## Description

<div><p>Consider an array of integers $C = [c_1, c_2, \ldots, c_n]$ of length $n$. Let's build the sequence of arrays $D_0, D_1, D_2, \ldots, D_{n}$ of length $n+1$ in the following way:</p><ul> <li> The first element of this sequence will be equals $C$: $D_0 = C$. </li><li> For each $1 \leq i \leq n$ array $D_i$ will be constructed from $D_{i-1}$ in the following way: <ul> <li> Let's find the lexicographically smallest subarray of $D_{i-1}$ of length $i$. Then, the first $n-i$ elements of $D_i$ will be equals to the corresponding $n-i$ elements of array $D_{i-1}$ and the last $i$ elements of $D_i$ will be equals to the corresponding elements of the found subarray of length $i$. </li></ul> </li></ul><p>Array $x$ is subarray of array $y$, if $x$ can be obtained by deletion of several (possibly, zero or all) elements from the beginning of $y$ and several (possibly, zero or all) elements from the end of $y$.</p><p>For array $C$ let's denote array $D_n$ as $op(C)$.</p><p>Alice has an array of integers $A = [a_1, a_2, \ldots, a_n]$ of length $n$. She will build the sequence of arrays $B_0, B_1, \ldots, B_n$ of length $n+1$ in the following way:</p><ul> <li> The first element of this sequence will be equals $A$: $B_0 = A$. </li><li> For each $1 \leq i \leq n$ array $B_i$ will be equals $op(B_{i-1})$, where $op$ is the transformation described above. </li></ul><p>She will ask you $q$ queries about elements of sequence of arrays $B_0, B_1, \ldots, B_n$. Each query consists of two integers $i$ and $j$, and the answer to this query is the value of the $j$-th element of array $B_i$.</p></div><div class="input-specification"><p>The first line contains the single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the length of array $A$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$)&nbsp;— the array $A$.</p><p>The third line contains the single integer $q$ ($1 \leq q \leq 10^6$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contains two integers $i$, $j$ ($1 \leq i, j \leq n$)&nbsp;— parameters of queries.</p></div><div class="output-specification"><p>Output $q$ integers: values of $B_{i, j}$ for required $i$, $j$.</p></div>

## Input

<p>The first line contains the single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the length of array $A$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$)&nbsp;— the array $A$.</p><p>The third line contains the single integer $q$ ($1 \leq q \leq 10^6$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contains two integers $i$, $j$ ($1 \leq i, j \leq n$)&nbsp;— parameters of queries.</p>

## Output

<p>Output $q$ integers: values of $B_{i, j}$ for required $i$, $j$.</p>





```input1
4
2 1 3 1
4
1 1
1 2
1 3
1 4
```




```output1
2
1
1
3
```



## Note

<p>In the first test case $B_0 = A = [2, 1, 3, 1]$.</p><p>$B_1$ is constructed in the following way:</p><ul> <li> Initially, $D_0 = [2, 1, 3, 1]$. </li><li> For $i=1$ the lexicographically smallest subarray of $D_0$ of length $1$ is $[1]$, so $D_1$ will be $[2, 1, 3, 1]$. </li><li> For $i=2$ the lexicographically smallest subarray of $D_1$ of length $2$ is $[1, 3]$, so $D_2$ will be $[2, 1, 1, 3]$. </li><li> For $i=3$ the lexicographically smallest subarray of $D_2$ of length $3$ is $[1, 1, 3]$, so $D_3$ will be $[2, 1, 1, 3]$. </li><li> For $i=4$ the lexicographically smallest subarray of $D_3$ of length $4$ is $[2, 1, 1, 3]$, so $D_4$ will be $[2, 1, 1, 3]$. </li><li> So, $B_1 = op(B_0) = op([2, 1, 3, 1]) = [2, 1, 1, 3]$. </li></ul>
