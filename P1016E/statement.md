## Description

<div><p>There is a light source on the plane. This source is so small that it can be represented as point. The light source is moving from point $(a, s_y)$ to the $(b, s_y)$ $(s_y &lt; 0)$ with speed equal to $1$ unit per second. The trajectory of this light source is a straight segment connecting these two points. </p><p>There is also a fence on $OX$ axis represented as $n$ segments $(l_i, r_i)$ (so the actual coordinates of endpoints of each segment are $(l_i, 0)$ and $(r_i, 0)$). The point $(x, y)$ is <span class="tex-font-style-it">in the shade</span> if segment connecting $(x,y)$ and the current position of the light source intersects or touches with any segment of the fence.</p><center> <img class="tex-graphics" src="file://MWuN0c6g.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given $q$ points. For each point calculate total time of this point being in the shade, while the light source is moving from $(a, s_y)$ to the $(b, s_y)$.</p></div><div class="input-specification"><p>First line contains three space separated integers $s_y$, $a$ and $b$ ($-10^9 \le s_y &lt; 0$, $1 \le a &lt; b \le 10^9$) — corresponding coordinates of the light source.</p><p>Second line contains single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — number of segments in the fence.</p><p>Next $n$ lines contain two integers per line: $l_i$ and $r_i$ ($1 \le l_i &lt; r_i \le 10^9$, $r_{i - 1} &lt; l_i$) — segments in the fence in increasing order. Segments don't intersect or touch each other.</p><p>Next line contains single integer $q$ ($1 \le q \le 2 \cdot 10^5$) — number of points to check.</p><p>Next $q$ lines contain two integers per line: $x_i$ and $y_i$ ($1 \le x_i, y_i \le 10^9$) — points to process.</p></div><div class="output-specification"><p>Print $q$ lines. The $i$-th line should contain one real number — total time of the $i$-th point being in the shade, while the light source is moving from $(a, s_y)$ to the $(b, s_y)$. The answer is considered as correct if its absolute of relative error doesn't exceed $10^{-6}$.</p></div>

## Input

<p>First line contains three space separated integers $s_y$, $a$ and $b$ ($-10^9 \le s_y &lt; 0$, $1 \le a &lt; b \le 10^9$) — corresponding coordinates of the light source.</p><p>Second line contains single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — number of segments in the fence.</p><p>Next $n$ lines contain two integers per line: $l_i$ and $r_i$ ($1 \le l_i &lt; r_i \le 10^9$, $r_{i - 1} &lt; l_i$) — segments in the fence in increasing order. Segments don't intersect or touch each other.</p><p>Next line contains single integer $q$ ($1 \le q \le 2 \cdot 10^5$) — number of points to check.</p><p>Next $q$ lines contain two integers per line: $x_i$ and $y_i$ ($1 \le x_i, y_i \le 10^9$) — points to process.</p>

## Output

<p>Print $q$ lines. The $i$-th line should contain one real number — total time of the $i$-th point being in the shade, while the light source is moving from $(a, s_y)$ to the $(b, s_y)$. The answer is considered as correct if its absolute of relative error doesn't exceed $10^{-6}$.</p>





```input1
-3 1 6
2
2 4
6 7
5
3 1
1 3
6 1
6 4
7 6

```




```output1
5.000000000000000
3.000000000000000
0.000000000000000
1.500000000000000
2.000000000000000

```



## Note

<ul> <li> The 1-st point is always in the shade; </li><li> the 2-nd point is in the shade while light source is moving from $(3, -3)$ to $(6, -3)$; </li><li> the 3-rd point is in the shade while light source is at point $(6, -3)$. </li><li> the 4-th point is in the shade while light source is moving from $(1, -3)$ to $(2.5, -3)$ and at point $(6, -3)$; </li><li> the 5-th point is in the shade while light source is moving from $(1, -3)$ to $(2.5, -3)$ and from $(5.5, -3)$ to $(6, -3)$; </li></ul>
