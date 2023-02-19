## Description

<div><p>You are given a <span class="tex-font-style-bf">non-decreasing</span> array of <span class="tex-font-style-bf">non-negative</span> integers $a_1, a_2, \ldots, a_n$. Also you are given a positive integer $k$.</p><p>You want to find $m$ <span class="tex-font-style-bf">non-decreasing</span> arrays of <span class="tex-font-style-bf">non-negative</span> integers $b_1, b_2, \ldots, b_m$, such that:</p><ul> <li> The size of $b_i$ is equal to $n$ for all $1 \leq i \leq m$. </li><li> For all $1 \leq j \leq n$, $a_j = b_{1, j} + b_{2, j} + \ldots + b_{m, j}$. In the other word, array $a$ is the sum of arrays $b_i$. </li><li> The number of different elements in the array $b_i$ is at most $k$ for all $1 \leq i \leq m$. </li></ul><p>Find the minimum possible value of $m$, or report that there is no possible $m$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 100$): the number of test cases.</p><p>The first line of each test case contains two integers $n$, $k$ ($1 \leq n \leq 100$, $1 \leq k \leq n$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_1 \leq a_2 \leq \ldots \leq a_n \leq 100$, $a_n &gt; 0$).</p></div><div class="output-specification"><p>For each test case print a single integer: the minimum possible value of $m$. If there is no such $m$, print $-1$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 100$): the number of test cases.</p><p>The first line of each test case contains two integers $n$, $k$ ($1 \leq n \leq 100$, $1 \leq k \leq n$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_1 \leq a_2 \leq \ldots \leq a_n \leq 100$, $a_n &gt; 0$).</p>

## Output

<p>For each test case print a single integer: the minimum possible value of $m$. If there is no such $m$, print $-1$.</p>





```input1
6
4 1
0 0 0 1
3 1
3 3 3
11 3
0 1 2 2 3 3 3 4 4 4 4
5 3
1 2 3 4 5
9 4
2 2 3 5 7 11 13 13 17
10 7
0 1 1 2 3 3 4 5 5 6
```




```output1
-1
1
2
2
2
1
```



## Note

<p>In the first test case, there is no possible $m$, because all elements of all arrays should be equal to $0$. But in this case, it is impossible to get $a_4 = 1$ as the sum of zeros.</p><p>In the second test case, we can take $b_1 = [3, 3, 3]$. $1$ is the smallest possible value of $m$.</p><p>In the third test case, we can take $b_1 = [0, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2]$ and $b_2 = [0, 0, 1, 1, 1, 1, 1, 2, 2, 2, 2]$. It's easy to see, that $a_i = b_{1, i} + b_{2, i}$ for all $i$ and the number of different elements in $b_1$ and in $b_2$ is equal to $3$ (so it is at most $3$). It can be proven that $2$ is the smallest possible value of $m$.</p>
