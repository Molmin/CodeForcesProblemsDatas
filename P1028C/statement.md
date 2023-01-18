## Description

<div><p>You are given $n$ rectangles on a plane with coordinates of their bottom left and upper right points. Some $(n-1)$ of the given $n$ rectangles have some common point. A point belongs to a rectangle if this point is strictly inside the rectangle or belongs to its boundary.</p><p>Find any point with integer coordinates that belongs to at least $(n-1)$ given rectangles.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 132\,674$) — the number of given rectangles.</p><p>Each the next $n$ lines contains four integers $x_1$, $y_1$, $x_2$ and $y_2$ ($-10^9 \le x_1 &lt; x_2 \le 10^9$, $-10^9 \le y_1 &lt; y_2 \le 10^9$) — the coordinates of the bottom left and upper right corners of a rectangle.</p></div><div class="output-specification"><p>Print two integers $x$ and $y$ — the coordinates of any point that belongs to at least $(n-1)$ given rectangles.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 132\,674$) — the number of given rectangles.</p><p>Each the next $n$ lines contains four integers $x_1$, $y_1$, $x_2$ and $y_2$ ($-10^9 \le x_1 &lt; x_2 \le 10^9$, $-10^9 \le y_1 &lt; y_2 \le 10^9$) — the coordinates of the bottom left and upper right corners of a rectangle.</p>

## Output

<p>Print two integers $x$ and $y$ — the coordinates of any point that belongs to at least $(n-1)$ given rectangles.</p>





```input1
3
0 0 1 1
1 1 2 2
3 0 4 1

```




```input2
3
0 0 1 1
0 1 1 2
1 0 2 1

```




```input3
4
0 0 5 5
0 0 4 4
1 1 4 4
1 1 4 4

```




```input4
5
0 0 10 8
1 2 6 7
2 3 5 6
3 4 4 5
8 1 9 2

```




```output1
1 1

```




```output2
1 1

```




```output3
1 1

```




```output4
3 4

```



## Note

<p>The picture below shows the rectangles in the first and second samples. The possible answers are highlighted.</p><center> <img class="tex-graphics" height="138px" src="file://TiVwgEDJ.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>The picture below shows the rectangles in the third and fourth samples.</p><center> <img class="tex-graphics" height="273px" src="file://GQciMEoj.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center>
