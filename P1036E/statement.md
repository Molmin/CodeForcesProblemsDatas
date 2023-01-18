## Description

<div><p>You are given $n$ segments on a Cartesian plane. Each segment's endpoints have integer coordinates. Segments can intersect with each other. No two segments lie on the same line.</p><p>Count the number of distinct points with <span class="tex-font-style-bf">integer coordinates</span>, which are covered by at least one segment.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 1000$) — the number of segments.</p><p>Each of the next $n$ lines contains four integers $Ax_i, Ay_i, Bx_i, By_i$ ($-10^6 \le Ax_i, Ay_i, Bx_i, By_i \le 10^6$) — the coordinates of the endpoints $A$, $B$ ($A \ne B$) of the $i$-th segment.</p><p>It is guaranteed that no two segments lie on the same line.</p></div><div class="output-specification"><p>Print a single integer — the number of distinct points with integer coordinates, which are covered by at least one segment.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 1000$) — the number of segments.</p><p>Each of the next $n$ lines contains four integers $Ax_i, Ay_i, Bx_i, By_i$ ($-10^6 \le Ax_i, Ay_i, Bx_i, By_i \le 10^6$) — the coordinates of the endpoints $A$, $B$ ($A \ne B$) of the $i$-th segment.</p><p>It is guaranteed that no two segments lie on the same line.</p>

## Output

<p>Print a single integer — the number of distinct points with integer coordinates, which are covered by at least one segment.</p>





```input1
9
0 0 4 4
-1 5 4 0
4 0 4 4
5 2 11 2
6 1 6 7
5 6 11 6
10 1 10 7
7 0 9 8
10 -1 11 -1

```




```input2
4
-1 2 1 2
-1 0 1 0
-1 0 0 3
0 3 1 0

```




```output1
42

```




```output2
7

```



## Note

<p>The image for the first example:</p><center> <img class="tex-graphics" src="file://DtMWO9Rb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Several key points are marked blue, the answer contains some non-marked points as well.</p><p>The image for the second example:</p><center> <img class="tex-graphics" src="file://BNTA6NDb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
