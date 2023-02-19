## Description

<div><p>We are given a rooted tree consisting of $n$ vertices numbered from $1$ to $n$. The root of the tree is the vertex $1$ and the parent of the vertex $v$ is $p_v$.</p><p>There is a number written on each vertex, initially all numbers are equal to $0$. Let's denote the number written on the vertex $v$ as $a_v$.</p><p>For each $v$, we want $a_v$ to be between $l_v$ and $r_v$ $(l_v \leq a_v \leq r_v)$.</p><p>In a single operation we do the following: </p><ul> <li> Choose some vertex $v$. Let $b_1, b_2, \ldots, b_k$ be vertices on the path from the vertex $1$ to vertex $v$ (meaning $b_1 = 1$, $b_k = v$ and $b_i = p_{b_{i + 1}}$).</li><li> Choose a non-decreasing array $c$ of length $k$ of nonnegative integers: $0 \leq c_1 \leq c_2 \leq \ldots \leq c_k$.</li><li> For each $i$ $(1 \leq i \leq k)$, increase $a_{b_i}$ by $c_i$. </li></ul><p>What's the minimum number of operations needed to achieve our goal?</p></div><div class="input-specification"><p>The first line contains an integer $t$ $(1\le t\le 1000)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2\le n\le 2 \cdot 10^5)$ &nbsp;— the number of the vertices in the tree.</p><p>The second line of each test case contains $n - 1$ integers, $p_2, p_3, \ldots, p_n$ $(1 \leq p_i &lt; i)$, where $p_i$ denotes the parent of the vertex $i$.</p><p>The $i$-th of the following $n$ lines contains two integers $l_i$ and $r_i$ $(1 \le l_i \le r_i \le 10^9)$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output the minimum number of operations needed.</p></div>

## Input

<p>The first line contains an integer $t$ $(1\le t\le 1000)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2\le n\le 2 \cdot 10^5)$ &nbsp;— the number of the vertices in the tree.</p><p>The second line of each test case contains $n - 1$ integers, $p_2, p_3, \ldots, p_n$ $(1 \leq p_i &lt; i)$, where $p_i$ denotes the parent of the vertex $i$.</p><p>The $i$-th of the following $n$ lines contains two integers $l_i$ and $r_i$ $(1 \le l_i \le r_i \le 10^9)$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output the minimum number of operations needed.</p>





```input1|2,3,4,5,11,12,13,14,15,16
4
2
1
1 5
2 9
3
1 1
4 5
2 4
6 10
4
1 2 1
6 9
5 6
4 5
2 4
5
1 2 3 4
5 5
4 4
3 3
2 2
1 1
```




```output1
1
2
2
5
```



## Note

<p>In the first test case, we can achieve the goal with a single operation: choose $v = 2$ and $c = [1, 2]$, resulting in $a_1 = 1, a_2 = 2$.</p><p>In the second test case, we can achieve the goal with two operations: first, choose $v = 2$ and $c = [3, 3]$, resulting in $a_1 = 3, a_2 = 3, a_3 = 0$. Then, choose $v = 3, c = [2, 7]$, resulting in $a_1 = 5, a_2 = 3, a_3 = 7$.</p>
