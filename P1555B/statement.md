## Description

<div><p>You have an axis-aligned rectangle room with width $W$ and height $H$, so the lower left corner is in point $(0, 0)$ and the upper right corner is in $(W, H)$.</p><p>There is a rectangular table standing in this room. The sides of the table are parallel to the walls, the lower left corner is in $(x_1, y_1)$, and the upper right corner in $(x_2, y_2)$.</p><p>You want to place another rectangular table in this room with width $w$ and height $h$ with the width of the table parallel to the width of the room.</p><p>The problem is that sometimes there is not enough space to place the second table without intersecting with the first one (there are no problems with tables touching, though).</p><p>You <span class="tex-font-style-bf">can't rotate</span> any of the tables, but you can move the first table inside the room. </p><center> <img class="tex-graphics" src="file://VYk9zDWt.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Example of how you may move the first table.</span> </center><p>What is the minimum distance you should move the first table to free enough space for the second one?</p></div><div class="input-specification"><p>The first line contains the single integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of the test cases.</p><p>The first line of each test case contains two integers $W$ and $H$ ($1 \le W, H \le 10^8$)&nbsp;— the width and the height of the room.</p><p>The second line contains four integers $x_1$, $y_1$, $x_2$ and $y_2$ ($0 \le x_1 &lt; x_2 \le W$; $0 \le y_1 &lt; y_2 \le H$)&nbsp;— the coordinates of the corners of the first table.</p><p>The third line contains two integers $w$ and $h$ ($1 \le w \le W$; $1 \le h \le H$)&nbsp;— the width and the height of the second table.</p></div><div class="output-specification"><p>For each test case, print the minimum distance you should move the first table, or $-1$ if there is no way to free enough space for the second table.</p><p>Your answer will be considered correct if its absolute or relative error doesn't exceed $10^{-6}$.</p></div>

## Input

<p>The first line contains the single integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of the test cases.</p><p>The first line of each test case contains two integers $W$ and $H$ ($1 \le W, H \le 10^8$)&nbsp;— the width and the height of the room.</p><p>The second line contains four integers $x_1$, $y_1$, $x_2$ and $y_2$ ($0 \le x_1 &lt; x_2 \le W$; $0 \le y_1 &lt; y_2 \le H$)&nbsp;— the coordinates of the corners of the first table.</p><p>The third line contains two integers $w$ and $h$ ($1 \le w \le W$; $1 \le h \le H$)&nbsp;— the width and the height of the second table.</p>

## Output

<p>For each test case, print the minimum distance you should move the first table, or $-1$ if there is no way to free enough space for the second table.</p><p>Your answer will be considered correct if its absolute or relative error doesn't exceed $10^{-6}$.</p>





```input1
5
8 5
2 1 7 4
4 2
5 4
2 2 5 4
3 3
1 8
0 3 1 6
1 5
8 1
3 0 6 1
5 1
8 10
4 5 7 8
8 5
```




```output1
1.000000000
-1
2.000000000
2.000000000
0.000000000
```



## Note

<p>The configuration of the first test case is shown in the picture. But the movement of the first table is not optimal. One of the optimal movement, for example, is to move the table by $(0, -1)$, so the lower left corner will move from $(2, 1)$ to $(2, 0)$. Then you can place the second table at $(0, 3)-(4, 5)$.</p><p>In the second test case, there is no way to fit both tables in the room without intersecting.</p><p>In the third test case, you can move the first table by $(0, 2)$, so the lower left corner will move from $(0, 3)$ to $(0, 5)$.</p>
