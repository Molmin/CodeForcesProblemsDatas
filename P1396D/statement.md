## Description

<div><p>Shrimpy Duc is a fat and greedy boy who is always hungry. After a while of searching for food to satisfy his never-ending hunger, Shrimpy Duc finds M&amp;M candies lying unguarded on a $L \times L$ grid. There are $n$ M&amp;M candies on the grid, the $i$-th M&amp;M is currently located at $(x_i + 0.5, y_i + 0.5),$ and has color $c_i$ out of a total of $k$ colors (the size of M&amp;Ms are insignificant).</p><p>Shrimpy Duc wants to steal a <span class="tex-font-style-bf">rectangle</span> of M&amp;Ms, specifically, he wants to select a rectangle with <span class="tex-font-style-bf">integer</span> coordinates within the grid and steal all candies within the rectangle. Shrimpy Duc doesn't need to steal every single candy, however, he would like to steal <span class="tex-font-style-bf">at least one candy for each color</span>.</p><p>In other words, he wants to select a rectangle whose sides are parallel to the coordinate axes and whose left-bottom vertex $(X_1, Y_1)$ and right-top vertex $(X_2, Y_2)$ are points with integer coordinates satisfying $0 \le X_1 &lt; X_2 \le L$ and $0 \le Y_1 &lt; Y_2 \le L$, so that for every color $1 \le c \le k$ there is at least one M&amp;M with color $c$ that lies within that rectangle.</p><p>How many such rectangles are there? This number may be large, so you only need to find it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains three positive integers $n, k, L$ $(1 \leq k \leq n \leq 2 \cdot 10^3, 1 \leq L \leq 10^9 )$ — the number of M&amp;Ms, the number of colors and the length of the grid respectively.</p><p>The following $n$ points describe the M&amp;Ms. Each line contains three integers $x_i, y_i, c_i$ $(0 \leq x_i, y_i &lt; L, 1 \le c_i \le k)$ — the coordinates and color of the $i$-th M&amp;M respectively. </p><p>Different M&amp;Ms have different coordinates ($x_i \ne x_j$ or $y_i \ne y_j$ for every $i \ne j$), and for every $1 \le c \le k$ there is at least one M&amp;M with color $c$.</p></div><div class="output-specification"><p>Output a single integer — the number of rectangles satisfying Shrimpy Duc's conditions, modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains three positive integers $n, k, L$ $(1 \leq k \leq n \leq 2 \cdot 10^3, 1 \leq L \leq 10^9 )$ — the number of M&amp;Ms, the number of colors and the length of the grid respectively.</p><p>The following $n$ points describe the M&amp;Ms. Each line contains three integers $x_i, y_i, c_i$ $(0 \leq x_i, y_i &lt; L, 1 \le c_i \le k)$ — the coordinates and color of the $i$-th M&amp;M respectively. </p><p>Different M&amp;Ms have different coordinates ($x_i \ne x_j$ or $y_i \ne y_j$ for every $i \ne j$), and for every $1 \le c \le k$ there is at least one M&amp;M with color $c$.</p>

## Output

<p>Output a single integer — the number of rectangles satisfying Shrimpy Duc's conditions, modulo $10^9 + 7$.</p>





```input1
4 2 4
3 2 2
3 1 1
1 1 1
1 2 1
```




```input2
5 3 10
6 5 3
5 3 1
7 9 1
2 3 2
5 0 2
```




```input3
10 4 10
5 4 4
0 0 3
6 0 1
3 9 2
8 7 1
8 1 3
2 1 3
6 3 2
3 5 3
4 3 4
```




```output1
20
```




```output2
300
```




```output3
226
```



## Note

<p>Grid for the first sample:</p><p><img class="tex-graphics" src="file://2oRoYIHN.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
