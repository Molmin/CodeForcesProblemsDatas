## Description

<div><p><span class="tex-font-style-bf">This version of the problem differs from the next one only in the constraint on $n$</span>.</p><p>A tree is a connected undirected graph without cycles. A weighted tree has a weight assigned to each edge. The distance between two vertices is the minimum sum of weights on the path connecting them.</p><p>You are given a weighted tree with $n$ vertices, each edge has a weight of $1$. Denote $d(v)$ as the distance between vertex $1$ and vertex $v$.</p><p>Let $f(x)$ be the minimum possible value of $\max\limits_{1 \leq v \leq n} \ {d(v)}$ if you can temporarily add an edge with weight $x$ between any two vertices $a$ and $b$ $(1 \le a, b \le n)$. Note that after this operation, the graph is no longer a tree.</p><p>For each integer $x$ from $1$ to $n$, find $f(x)$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 3000$).</p><p>Each of the next $n−1$ lines contains two integers $u$ and $v$ ($1 \le u,v \le n$) indicating that there is an edge between vertices $u$ and $v$. It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3000$.</p></div><div class="output-specification"><p>For each test case, print $n$ integers in a single line, $x$-th of which is equal to $f(x)$ for all $x$ from $1$ to $n$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 3000$).</p><p>Each of the next $n−1$ lines contains two integers $u$ and $v$ ($1 \le u,v \le n$) indicating that there is an edge between vertices $u$ and $v$. It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3000$.</p>

## Output

<p>For each test case, print $n$ integers in a single line, $x$-th of which is equal to $f(x)$ for all $x$ from $1$ to $n$.</p>





```input1|2,3,4,5,8,9,10,11,12,13,14
3
4
1 2
2 3
1 4
2
1 2
7
1 2
1 3
3 4
3 5
3 6
5 7
```




```output1
1 2 2 2 
1 1 
2 2 3 3 3 3 3
```



## Note

<center> <img class="tex-graphics" src="file://GWB6XX8j.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> In the first testcase: <ul> <li> For $x = 1$, we can an edge between vertices $1$ and $3$, then $d(1) = 0$ and $d(2) = d(3) = d(4) = 1$, so $f(1) = 1$. </li><li> For $x \ge 2$, no matter which edge we add, $d(1) = 0$, $d(2) = d(4) = 1$ and $d(3) = 2$, so $f(x) = 2$. </li></ul>
