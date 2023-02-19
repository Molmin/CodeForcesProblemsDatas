## Description

<div><p>You are given three points on a plane. You should choose some segments on the plane that are parallel to coordinate axes, so that all three points become connected. The total length of the chosen segments should be the minimal possible.</p><p>Two points $a$ and $b$ are considered connected if there is a sequence of points $p_0 = a, p_1, \ldots, p_k = b$ such that points $p_i$ and $p_{i+1}$ lie on the same segment.</p></div><div class="input-specification"><p>The input consists of three lines describing three points. Each line contains two integers $x$ and $y$ separated by a space&nbsp;— the coordinates of the point ($-10^9 \le x, y \le 10^9$). The points are pairwise distinct.</p></div><div class="output-specification"><p>On the first line output $n$&nbsp;— the number of segments, at most 100.</p><p>The next $n$ lines should contain descriptions of segments. Output four integers $x_1$, $y_1$, $x_2$, $y_2$ on a line&nbsp;— the coordinates of the endpoints of the corresponding segment ($-10^9 \le x_1, y_1, x_2, y_2 \le 10^9$). Each segment should be either horizontal or vertical.</p><p>It is guaranteed that the solution with the given constraints exists.</p></div>

## Input

<p>The input consists of three lines describing three points. Each line contains two integers $x$ and $y$ separated by a space&nbsp;— the coordinates of the point ($-10^9 \le x, y \le 10^9$). The points are pairwise distinct.</p>

## Output

<p>On the first line output $n$&nbsp;— the number of segments, at most 100.</p><p>The next $n$ lines should contain descriptions of segments. Output four integers $x_1$, $y_1$, $x_2$, $y_2$ on a line&nbsp;— the coordinates of the endpoints of the corresponding segment ($-10^9 \le x_1, y_1, x_2, y_2 \le 10^9$). Each segment should be either horizontal or vertical.</p><p>It is guaranteed that the solution with the given constraints exists.</p>





```input1
1 1
3 5
8 6
```




```output1
3
1 1 1 5
1 5 8 5
8 5 8 6
```



## Note

<p>The points and the segments from the example are shown below.</p><center> <img class="tex-graphics" src="file://E5xEItlI.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
