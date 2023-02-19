## Description

<div><p>You are given $n$ colored segments on the number line. Each segment is either colored red or blue. The $i$-th segment can be represented by a tuple $(c_i, l_i, r_i)$. The segment contains all the points in the range $[l_i, r_i]$, inclusive, and its color denoted by $c_i$: </p><ul> <li> if $c_i = 0$, it is a red segment; </li><li> if $c_i = 1$, it is a blue segment. </li></ul><p>We say that two segments of <span class="tex-font-style-bf">different</span> colors are <span class="tex-font-style-it">connected</span>, if they share at least one common point. Two segments belong to the same group, if they are either connected directly, or through a sequence of directly connected segments. Find the number of groups of segments.</p><center> <img class="tex-graphics" src="file://xf7WxfrQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> </div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the number of segments. </p><p>Each of the next $n$ lines contains three integers $c_i, l_i, r_i$ ($0 \leq c_i \leq 1, 0 \leq l_i \leq r_i \leq 10^9$), describing the $i$-th segment. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer $k$, the number of groups of segments.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the number of segments. </p><p>Each of the next $n$ lines contains three integers $c_i, l_i, r_i$ ($0 \leq c_i \leq 1, 0 \leq l_i \leq r_i \leq 10^9$), describing the $i$-th segment. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print a single integer $k$, the number of groups of segments.</p>





```input1
2
5
0 0 5
1 2 12
0 4 7
1 9 16
0 13 19
3
1 0 1
1 1 2
0 3 4
```




```output1
2
3
```



## Note

<p>In the first example there are $5$ segments. The segments $1$ and $2$ are connected, because they are of different colors and share a point. Also, the segments $2$ and $3$ are connected, and so are segments $4$ and $5$. Thus, there are two groups: one containing segments $\{1, 2, 3\}$, and the other one containing segments $\{4, 5\}$.</p>
