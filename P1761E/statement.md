## Description

<div><p>You are given a simple undirected graph consisting of $n$ vertices. The graph doesn't contain self-loops, there is at most one edge between each pair of vertices. Your task is simple: make the graph connected.</p><p>You can do the following operation any number of times (possibly zero):</p><ul> <li> Choose a vertex $u$ arbitrarily. </li><li> For each vertex $v$ satisfying $v\ne u$ in the graph individually, if $v$ is adjacent to $u$, remove the edge between $u$ and $v$, otherwise add an edge between $u$ and $v$. </li></ul><p>Find the minimum number of operations required to make the graph connected. Also, find any sequence of operations with the minimum length that makes the graph connected.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1\leq t\leq 800$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2\leq n\leq 4000$)&nbsp;— the number of vertices in the graph.</p><p>Then $n$ lines follow. The $i$-th row contains a binary string $s_i$ of length $n$, where $s_{i,j}$ is '<span class="tex-font-style-tt">1</span>' if there is an edge between vertex $i$ and $j$ initially, otherwise $s_{i,j}$ is '<span class="tex-font-style-tt">0</span>'.</p><p>It is guaranteed that $s_{i,i}$ is always '<span class="tex-font-style-tt">0</span>' and $s_{i,j}=s_{j,i}$ for $1\leq i,j\leq n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $4000$.</p></div><div class="output-specification"><p>For each test case, in the first line, output an integer $m$ &nbsp;— the minimum number of operations required.</p><p>If $m$ is greater than zero, then print an extra line consisting of $m$ integers&nbsp;— the vertices chosen in the operations in your solution. If there are multiple solutions with the minimum number of operations, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1\leq t\leq 800$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2\leq n\leq 4000$)&nbsp;— the number of vertices in the graph.</p><p>Then $n$ lines follow. The $i$-th row contains a binary string $s_i$ of length $n$, where $s_{i,j}$ is '<span class="tex-font-style-tt">1</span>' if there is an edge between vertex $i$ and $j$ initially, otherwise $s_{i,j}$ is '<span class="tex-font-style-tt">0</span>'.</p><p>It is guaranteed that $s_{i,i}$ is always '<span class="tex-font-style-tt">0</span>' and $s_{i,j}=s_{j,i}$ for $1\leq i,j\leq n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $4000$.</p>

## Output

<p>For each test case, in the first line, output an integer $m$ &nbsp;— the minimum number of operations required.</p><p>If $m$ is greater than zero, then print an extra line consisting of $m$ integers&nbsp;— the vertices chosen in the operations in your solution. If there are multiple solutions with the minimum number of operations, print any.</p>





```input1|2,3,4,5,10,11,12,13,14
4
3
011
100
100
3
000
001
010
4
0100
1000
0001
0010
6
001100
000011
100100
101000
010001
010010
```




```output1
0
1
1
2
3 4 
3
2 5 6
```



## Note

<p>In the first test case, the graph is connected at the beginning, so the answer is $0$.</p><p>In the second test case, if we do the operation with vertex $1$, we will get the following graph represented by an adjacency matrix:</p><p>$$ \begin{bmatrix} 0&amp;1&amp;1\\ 1&amp;0&amp;1\\ 1&amp;1&amp;0 \end{bmatrix} $$</p><p>It's obvious that the graph above is connected.</p><p>In the third test case, if we do the operation with vertex $3$ and $4$, we will get the following graph represented by an adjacency matrix:</p><p>$$ \begin{bmatrix} 0&amp;1&amp;1&amp;1\\ 1&amp;0&amp;1&amp;1\\ 1&amp;1&amp;0&amp;1\\ 1&amp;1&amp;1&amp;0 \end{bmatrix} $$</p><p>It's obvious that the graph above is connected, and it can be proven that we can't perform less than $2$ operations to make the graph connected.</p>
