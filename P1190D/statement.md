## Description

<div><p>There are $n$ points on the plane, the $i$-th of which is at $(x_i, y_i)$. Tokitsukaze wants to draw a strange rectangular area and pick all the points in the area.</p><p>The strange area is enclosed by three lines, $x = l$, $y = a$ and $x = r$, as its left side, its bottom side and its right side respectively, where $l$, $r$ and $a$ can be any real numbers satisfying that $l &lt; r$. The upper side of the area is boundless, which you can regard as a line parallel to the $x$-axis at infinity. The following figure shows a strange rectangular area.</p><center> <img class="tex-graphics" height="227px" src="file://jdpqV5c1.png" style="max-width: 100.0%;max-height: 100.0%;" width="284px"> </center><p>A point $(x_i, y_i)$ is in the strange rectangular area if and only if $l &lt; x_i &lt; r$ and $y_i &gt; a$. For example, in the above figure, $p_1$ is in the area while $p_2$ is not.</p><p>Tokitsukaze wants to know how many different non-empty sets she can obtain by picking all the points in a strange rectangular area, where we think two sets are different if there exists at least one point in one set of them but not in the other.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 2 \times 10^5$)&nbsp;— the number of points on the plane.</p><p>The $i$-th of the next $n$ lines contains two integers $x_i$, $y_i$ ($1 \leq x_i, y_i \leq 10^9$)&nbsp;— the coordinates of the $i$-th point.</p><p>All points are distinct.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of different non-empty sets of points she can obtain.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 2 \times 10^5$)&nbsp;— the number of points on the plane.</p><p>The $i$-th of the next $n$ lines contains two integers $x_i$, $y_i$ ($1 \leq x_i, y_i \leq 10^9$)&nbsp;— the coordinates of the $i$-th point.</p><p>All points are distinct.</p>

## Output

<p>Print a single integer&nbsp;— the number of different non-empty sets of points she can obtain.</p>





```input1
3
1 1
1 2
1 3

```




```input2
3
1 1
2 1
3 1

```




```input3
4
2 1
2 2
3 1
3 2

```




```output1
3

```




```output2
6

```




```output3
6

```



## Note

<p>For the first example, there is exactly one set having $k$ points for $k = 1, 2, 3$, so the total number is $3$.</p><p>For the second example, the numbers of sets having $k$ points for $k = 1, 2, 3$ are $3$, $2$, $1$ respectively, and their sum is $6$.</p><p>For the third example, as the following figure shows, there are</p><ul> <li> $2$ sets having one point; </li><li> $3$ sets having two points; </li><li> $1$ set having four points. </li></ul><p>Therefore, the number of different non-empty sets in this example is $2 + 3 + 0 + 1 = 6$.</p><center> <img class="tex-graphics" height="151px" src="file://o5DzqR21.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center>
