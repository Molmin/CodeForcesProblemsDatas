## Description

<div><p>Recently, Masha was presented with a chessboard with a height of $n$ and a width of $m$.</p><p>The rows on the chessboard are numbered from $1$ to $n$ from bottom to top. The columns are numbered from $1$ to $m$ from left to right. Therefore, each cell can be specified with the coordinates $(x,y)$, where $x$ is the <span class="tex-font-style-bf">column</span> number, and $y$ is the <span class="tex-font-style-bf">row</span> number <span class="tex-font-style-bf">(do not mix up)</span>.</p><p>Let us call a rectangle with coordinates $(a,b,c,d)$ a rectangle lower left point of which has coordinates $(a,b)$, and the upper right one&nbsp;— $(c,d)$.</p><p>The chessboard is painted black and white as follows:</p><center> <img class="tex-graphics" height="302px" src="file://w9Xhbttm.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center><center> <span class="tex-font-size-small">An example of a chessboard.</span> </center><p>Masha was very happy with the gift and, therefore, invited her friends Maxim and Denis to show off. The guys decided to make her a treat&nbsp;— they bought her a can of white and a can of black paint, so that if the old board deteriorates, it can be repainted. When they came to Masha, something unpleasant happened: first, Maxim went over the threshold and spilled <span class="tex-font-style-bf">white</span> paint on the rectangle $(x_1,y_1,x_2,y_2)$. Then after him Denis spilled <span class="tex-font-style-bf">black</span> paint on the rectangle $(x_3,y_3,x_4,y_4)$.</p><p>To spill paint of color $color$ onto a certain rectangle means that all the cells that belong to the given rectangle become $color$. The cell dyeing is superimposed on each other (if at first some cell is spilled with white paint and then with black one, then its color will be black).</p><p>Masha was shocked! She drove away from the guests and decided to find out how spoiled the gift was. For this, she needs to know the number of cells of white and black color. Help her find these numbers!</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^3$)&nbsp;— the number of test cases.</p><p>Each of them is described in the following format:</p><p>The first line contains two integers $n$ and $m$ ($1 \le n,m \le 10^9$)&nbsp;— the size of the board.</p><p>The second line contains four integers $x_1$, $y_1$, $x_2$, $y_2$ ($1 \le x_1 \le x_2 \le m, 1 \le y_1 \le y_2 \le n$)&nbsp;— the coordinates of the rectangle, the white paint was spilled on.</p><p>The third line contains four integers $x_3$, $y_3$, $x_4$, $y_4$ ($1 \le x_3 \le x_4 \le m, 1 \le y_3 \le y_4 \le n$)&nbsp;— the coordinates of the rectangle, the black paint was spilled on.</p></div><div class="output-specification"><p>Output $t$ lines, each of which contains two numbers&nbsp;— the number of white and black cells after spilling paint, respectively.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^3$)&nbsp;— the number of test cases.</p><p>Each of them is described in the following format:</p><p>The first line contains two integers $n$ and $m$ ($1 \le n,m \le 10^9$)&nbsp;— the size of the board.</p><p>The second line contains four integers $x_1$, $y_1$, $x_2$, $y_2$ ($1 \le x_1 \le x_2 \le m, 1 \le y_1 \le y_2 \le n$)&nbsp;— the coordinates of the rectangle, the white paint was spilled on.</p><p>The third line contains four integers $x_3$, $y_3$, $x_4$, $y_4$ ($1 \le x_3 \le x_4 \le m, 1 \le y_3 \le y_4 \le n$)&nbsp;— the coordinates of the rectangle, the black paint was spilled on.</p>

## Output

<p>Output $t$ lines, each of which contains two numbers&nbsp;— the number of white and black cells after spilling paint, respectively.</p>





```input1
5
2 2
1 1 2 2
1 1 2 2
3 4
2 2 3 2
3 1 4 3
1 5
1 1 5 1
3 1 5 1
4 4
1 1 4 2
1 3 4 4
3 4
1 2 4 2
2 1 3 3
```




```output1
0 4
3 9
2 3
8 8
4 8
```



## Note

<p>Explanation for examples:</p><p>The first picture of each illustration shows how the field looked before the dyes were spilled. The second picture of each illustration shows how the field looked after Maxim spoiled white dye (the rectangle on which the dye was spilled is highlighted with red). The third picture in each illustration shows how the field looked after Denis spoiled black dye (the rectangle on which the dye was spilled is highlighted with red).</p><p>In the first test, the paint on the field changed as follows:</p><center> <img class="tex-graphics" height="208px" src="file://8V5LIYzr.png" style="max-width: 100.0%;max-height: 100.0%;" width="416px"> </center><p>In the second test, the paint on the field changed as follows:</p><center> <img class="tex-graphics" height="189px" src="file://S9sbv60w.png" style="max-width: 100.0%;max-height: 100.0%;" width="756px"> </center><p>In the third test, the paint on the field changed as follows:</p><center> <img class="tex-graphics" height="302px" src="file://Fk89Ey61.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center><p>In the fourth test, the paint on the field changed as follows:</p><center> <img class="tex-graphics" height="302px" src="file://eCjjmnLC.png" style="max-width: 100.0%;max-height: 100.0%;" width="605px"> </center><p>In the fifth test, the paint on the field changed as follows:</p><center> <img class="tex-graphics" height="189px" src="file://tc6tI7Aj.png" style="max-width: 100.0%;max-height: 100.0%;" width="756px"> </center>
