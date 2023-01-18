## Description

<div><p>We had a really tough time generating tests for problem D. In order to prepare strong tests, we had to solve the following problem.</p><p>Given an undirected labeled tree consisting of $n$ vertices, find a set of segments such that:</p><ol> <li> both endpoints of each segment are integers from $1$ to $2n$, and each integer from $1$ to $2n$ should appear as an endpoint of exactly one segment; </li><li> all segments are non-degenerate; </li><li> for each pair $(i, j)$ such that $i \ne j$, $i \in [1, n]$ and $j \in [1, n]$, the vertices $i$ and $j$ are connected with an edge if and only if the segments $i$ and $j$ intersect, but neither segment $i$ is fully contained in segment $j$, nor segment $j$ is fully contained in segment $i$. </li></ol><p>Can you solve this problem too?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the number of vertices in the tree.</p><p>Then $n - 1$ lines follow, each containing two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$, $x_i \ne y_i$) denoting the endpoints of the $i$-th edge.</p><p>It is guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>Print $n$ pairs of integers, the $i$-th pair should contain two integers $l_i$ and $r_i$ ($1 \le l_i &lt; r_i \le 2n$) — the endpoints of the $i$-th segment. All $2n$ integers you print should be unique.</p><p>It is guaranteed that the answer always exists.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the number of vertices in the tree.</p><p>Then $n - 1$ lines follow, each containing two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$, $x_i \ne y_i$) denoting the endpoints of the $i$-th edge.</p><p>It is guaranteed that the given graph is a tree.</p>

## Output

<p>Print $n$ pairs of integers, the $i$-th pair should contain two integers $l_i$ and $r_i$ ($1 \le l_i &lt; r_i \le 2n$) — the endpoints of the $i$-th segment. All $2n$ integers you print should be unique.</p><p>It is guaranteed that the answer always exists.</p>





```input1
6
1 2
1 3
3 4
3 5
2 6
```




```input2
1
```




```output1
9 12
7 10
3 11
1 5
2 4
6 8
```




```output2
1 2
```


