## Description

<div><p><span class="tex-font-style-bf">The only difference between this problem and D2 is the bound on the size of the tree.</span></p><p>You are given an unrooted tree with $n$ vertices. There is some hidden vertex $x$ in that tree that you are trying to find.</p><p>To do this, you may ask $k$ queries $v_1, v_2, \ldots, v_k$ where the $v_i$ are vertices in the tree. After you are finished asking all of the queries, you are given $k$ numbers $d_1, d_2, \ldots, d_k$, where $d_i$ is the number of edges on the shortest path between $v_i$ and $x$. Note that you know which distance corresponds to which query.</p><p>What is the minimum $k$ such that there exists some queries $v_1, v_2, \ldots, v_k$ that let you always uniquely identify $x$ (no matter what $x$ is).</p><p>Note that you don't actually need to output these queries.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2000$) &nbsp;— the number of vertices in the tree.</p><p>Each of the next $n-1$ lines contains two integers $x$ and $y$ ($1 \le x, y \le n$), meaning there is an edges between vertices $x$ and $y$ in the tree.</p><p>It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case print a single nonnegative integer, the minimum number of queries you need, on its own line.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2000$) &nbsp;— the number of vertices in the tree.</p><p>Each of the next $n-1$ lines contains two integers $x$ and $y$ ($1 \le x, y \le n$), meaning there is an edges between vertices $x$ and $y$ in the tree.</p><p>It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2000$.</p>

## Output

<p>For each test case print a single nonnegative integer, the minimum number of queries you need, on its own line.</p>





```input1|2,5,6,7,8,9,10,11,12,13,14
3
1
2
1 2
10
2 4
2 1
5 7
3 10
8 6
6 1
1 3
4 7
9 6
```




```output1
0
1
2
```



## Note

<p>In the first test case, there is only one vertex, so you don't need any queries.</p><p>In the second test case, you can ask a single query about the node $1$. Then, if $x = 1$, you will get $0$, otherwise you will get $1$.</p>
