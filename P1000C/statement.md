## Description

<div><p>You are given $n$ segments on a coordinate line; each endpoint of every segment has integer coordinates. Some segments can degenerate to points. Segments can intersect with each other, be nested in each other or even coincide.</p><p>Your task is the following: for every $k \in [1..n]$, calculate the number of points with integer coordinates such that the number of segments that cover these points equals $k$. A segment with endpoints $l_i$ and $r_i$ covers point $x$ if and only if $l_i \le x \le r_i$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of segments.</p><p>The next $n$ lines contain segments. The $i$-th line contains a pair of integers $l_i, r_i$ ($0 \le l_i \le r_i \le 10^{18}$) — the endpoints of the $i$-th segment.</p></div><div class="output-specification"><p>Print $n$ space separated integers $cnt_1, cnt_2, \dots, cnt_n$, where $cnt_i$ is equal to the number of points such that the number of segments that cover these points equals to $i$.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of segments.</p><p>The next $n$ lines contain segments. The $i$-th line contains a pair of integers $l_i, r_i$ ($0 \le l_i \le r_i \le 10^{18}$) — the endpoints of the $i$-th segment.</p>

## Output

<p>Print $n$ space separated integers $cnt_1, cnt_2, \dots, cnt_n$, where $cnt_i$ is equal to the number of points such that the number of segments that cover these points equals to $i$.</p>





```input1
3
0 3
1 3
3 8

```




```input2
3
1 3
2 4
5 7

```




```output1
6 2 1 

```




```output2
5 2 0 

```



## Note

<p>The picture describing the first example:</p><p><img class="tex-graphics" src="file://1gHnCuWz.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Points with coordinates $[0, 4, 5, 6, 7, 8]$ are covered by one segment, points $[1, 2]$ are covered by two segments and point $[3]$ is covered by three segments.</p><p>The picture describing the second example:</p><p><img class="tex-graphics" src="file://VOzjLB8C.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Points $[1, 4, 5, 6, 7]$ are covered by one segment, points $[2, 3]$ are covered by two segments and there are no points covered by three segments.</p>
