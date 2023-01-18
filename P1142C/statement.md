## Description

<div><p>Recently Vasya learned that, given two points with different $x$ coordinates, you can draw through them exactly one parabola with equation of type $y = x^2 + bx + c$, where $b$ and $c$ are reals. Let's call such a parabola an $U$-shaped one.</p><p>Vasya drew several distinct points with integer coordinates on a plane and then drew an $U$-shaped parabola through each pair of the points that have different $x$ coordinates. The picture became somewhat messy, but Vasya still wants to count how many of the parabolas drawn don't have any drawn point inside their internal area. Help Vasya.</p><p>The internal area of an $U$-shaped parabola is the part of the plane that lies strictly above the parabola when the $y$ axis is directed upwards.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 100\,000$)&nbsp;— the number of points.</p><p>The next $n$ lines describe the points, the $i$-th of them contains two integers $x_i$ and $y_i$&nbsp;— the coordinates of the $i$-th point. It is guaranteed that all points are distinct and that the coordinates do not exceed $10^6$ by absolute value.</p></div><div class="output-specification"><p>In the only line print a single integer&nbsp;— the number of $U$-shaped parabolas that pass through at least two of the given points and do not contain any of the given points inside their internal area (excluding the parabola itself).</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 100\,000$)&nbsp;— the number of points.</p><p>The next $n$ lines describe the points, the $i$-th of them contains two integers $x_i$ and $y_i$&nbsp;— the coordinates of the $i$-th point. It is guaranteed that all points are distinct and that the coordinates do not exceed $10^6$ by absolute value.</p>

## Output

<p>In the only line print a single integer&nbsp;— the number of $U$-shaped parabolas that pass through at least two of the given points and do not contain any of the given points inside their internal area (excluding the parabola itself).</p>





```input1
3
-1 0
0 2
1 0
```




```input2
5
1 0
1 -1
0 -1
-1 0
-1 -1
```




```output1
2
```




```output2
1
```



## Note

<p>On the pictures below all $U$-shaped parabolas that pass through at least two given points are drawn for each of the examples. The $U$-shaped parabolas that do not have any given point inside their internal area are drawn in red. </p><center> <img class="tex-graphics" height="643px" src="file://2NkWKbDI.png" style="max-width: 100.0%;max-height: 100.0%;" width="756px"> The first example. </center><center> <img class="tex-graphics" height="605px" src="file://I8dLBfyf.png" style="max-width: 100.0%;max-height: 100.0%;" width="756px"> The second example. </center>
