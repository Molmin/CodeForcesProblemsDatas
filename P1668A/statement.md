## Description

<div><p>You are given a grid with $n$ rows and $m$ columns. Rows and columns are numbered from $1$ to $n$, and from $1$ to $m$. The intersection of the $a$-th row and $b$-th column is denoted by $(a, b)$. </p><p>Initially, you are standing in the top left corner $(1, 1)$. Your goal is to reach the bottom right corner $(n, m)$.</p><p>You can move in four directions from $(a, b)$: up to $(a-1, b)$, down to $(a+1, b)$, left to $(a, b-1)$ or right to $(a, b+1)$.</p><p>You cannot move in the same direction in two consecutive moves, and you cannot leave the grid. What is the minimum number of moves to reach $(n, m)$?</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^3$) — the number of the test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 10^9$) — the size of the grid.</p></div><div class="output-specification"><p>For each test case, print a single integer: $-1$ if it is impossible to reach $(n, m)$ under the given conditions, otherwise the minimum number of moves.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^3$) — the number of the test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 10^9$) — the size of the grid.</p>

## Output

<p>For each test case, print a single integer: $-1$ if it is impossible to reach $(n, m)$ under the given conditions, otherwise the minimum number of moves.</p>





```input1
6
1 1
2 1
1 3
4 2
4 6
10 5
```




```output1
0
1
-1
6
10
17
```



## Note

<p>Test case $1$: $n=1$, $m=1$, and initially you are standing in $(1, 1)$ so $0$ move is required to reach $(n, m) = (1, 1)$.</p><p>Test case $2$: you should go down to reach $(2, 1)$.</p><p>Test case $3$: it is impossible to reach $(1, 3)$ without moving right two consecutive times, or without leaving the grid.</p><p>Test case $4$: an optimal moving sequence could be: $(1, 1) \to (1, 2) \to (2, 2) \to (2, 1) \to (3, 1) \to (3, 2) \to (4, 2)$. It can be proved that this is the optimal solution. So the answer is $6$.</p>
