## Description

<div><p>You are given $n$ <span class="tex-font-style-bf">distinct</span> points $p_1, p_2, \ldots, p_n$ on the plane and a positive integer $R$. </p><p>Find the number of pairs of indices $(i, j)$ such that $1 \le i &lt; j \le n$, and for every possible $k$ ($1 \le k \le n$) the distance from the point $p_k$ to the <span class="tex-font-style-bf">segment</span> between points $p_i$ and $p_j$ is at most $R$.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $R$ ($1 \le n \le 3000$, $1 \le R \le 10^5$)&nbsp;— the number of points and the maximum distance between a point and a segment.</p><p>Each of the next $n$ lines contains two integers $x_i$, $y_i$ ($-10^5 \le x_i, y_i \le 10^5$) that define the $i$-th point $p_i=(x_i, y_i)$. All points are distinct.</p><p>It is guaranteed that the answer does not change if the parameter $R$ is changed by at most $10^{-2}$.</p></div><div class="output-specification"><p>Print the number of suitable pairs $(i, j)$.</p></div>

## Input

<p>The first line contains two integers $n$, $R$ ($1 \le n \le 3000$, $1 \le R \le 10^5$)&nbsp;— the number of points and the maximum distance between a point and a segment.</p><p>Each of the next $n$ lines contains two integers $x_i$, $y_i$ ($-10^5 \le x_i, y_i \le 10^5$) that define the $i$-th point $p_i=(x_i, y_i)$. All points are distinct.</p><p>It is guaranteed that the answer does not change if the parameter $R$ is changed by at most $10^{-2}$.</p>

## Output

<p>Print the number of suitable pairs $(i, j)$.</p>





```input1
4 2
0 1
0 -1
3 0
-3 0
```




```input2
3 3
1 -1
-1 -1
0 1
```




```output1
1
```




```output2
3
```



## Note

<p>In the first example, the only pair of points $(-3, 0)$, $(3, 0)$ is suitable. The distance to the segment between these points from the points $(0, 1)$ and $(0, -1)$ is equal to $1$, which is less than $R=2$.</p><p>In the second example, all possible pairs of points are eligible.</p>
