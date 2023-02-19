## Description

<div><p>There are $n$ weighted points on the $OX$-axis. The coordinate and the weight of the $i$-th point is $x_i$ and $w_i$, respectively. All points have distinct coordinates and positive weights. Also, $x_i &lt; x_{i + 1}$ holds for any $1 \leq i &lt; n$. </p><p>The weighted distance between $i$-th point and $j$-th point is defined as $|x_i - x_j| \cdot (w_i + w_j)$, where $|val|$ denotes the absolute value of $val$.</p><p>You should answer $q$ queries, where the $i$-th query asks the following: Find the <span class="tex-font-style-bf">minimum</span> weighted distance among all pairs of distinct points among the points in subarray $[l_i,r_i]$.</p></div><div class="input-specification"><p>The first line contains 2 integers $n$ and $q$ $(2 \leq n \leq 3 \cdot 10^5; 1 \leq q \leq 3 \cdot 10^5)$ — the number of points and the number of queries.</p><p>Then, $n$ lines follows, the $i$-th of them contains two integers $x_i$ and $w_i$ $(-10^9 \leq x_i \leq 10^9; 1 \leq w_i \leq 10^9)$ — the coordinate and the weight of the $i$-th point.</p><p>It is guaranteed that the points are given in the increasing order of $x$.</p><p>Then, $q$ lines follows, the $i$-th of them contains two integers $l_i$ and $r_i$ $(1 \leq l_i &lt; r_i \leq n)$ — the given subarray of the $i$-th query.</p></div><div class="output-specification"><p>For each query output one integer, the <span class="tex-font-style-bf">minimum</span> weighted distance among all pair of distinct points in the given subarray.</p></div>

## Input

<p>The first line contains 2 integers $n$ and $q$ $(2 \leq n \leq 3 \cdot 10^5; 1 \leq q \leq 3 \cdot 10^5)$ — the number of points and the number of queries.</p><p>Then, $n$ lines follows, the $i$-th of them contains two integers $x_i$ and $w_i$ $(-10^9 \leq x_i \leq 10^9; 1 \leq w_i \leq 10^9)$ — the coordinate and the weight of the $i$-th point.</p><p>It is guaranteed that the points are given in the increasing order of $x$.</p><p>Then, $q$ lines follows, the $i$-th of them contains two integers $l_i$ and $r_i$ $(1 \leq l_i &lt; r_i \leq n)$ — the given subarray of the $i$-th query.</p>

## Output

<p>For each query output one integer, the <span class="tex-font-style-bf">minimum</span> weighted distance among all pair of distinct points in the given subarray.</p>





```input1
5 5
-2 2
0 10
1 1
9 2
12 7
1 3
2 3
1 5
3 5
2 4
```




```output1
9
11
9
24
11
```



## Note

<p>For the first query, the minimum weighted distance is between points $1$ and $3$, which is equal to $|x_1 - x_3| \cdot (w_1 + w_3) = |-2 - 1| \cdot (2 + 1) = 9$.</p><p>For the second query, the minimum weighted distance is between points $2$ and $3$, which is equal to $|x_2 - x_3| \cdot (w_2 + w_3) = |0 - 1| \cdot (10 + 1) = 11$.</p><p>For the fourth query, the minimum weighted distance is between points $3$ and $4$, which is equal to $|x_3 - x_4| \cdot (w_3 + w_4) = |1 - 9| \cdot (1 + 2) = 24$.</p>
