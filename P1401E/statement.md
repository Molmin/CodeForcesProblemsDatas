## Description

<div><p>There is a square of size $10^6 \times 10^6$ on the coordinate plane with four points $(0, 0)$, $(0, 10^6)$, $(10^6, 0)$, and $(10^6, 10^6)$ as its vertices.</p><p>You are going to draw segments on the plane. All segments are either horizontal or vertical and <span class="tex-font-style-it">intersect with at least one side of the square</span>.</p><p>Now you are wondering how many pieces this square divides into after drawing all segments. Write a program calculating the number of pieces of the square.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($0 \le n, m \le 10^5$)&nbsp;— the number of horizontal segments and the number of vertical segments.</p><p>The next $n$ lines contain descriptions of the horizontal segments. The $i$-th line contains three integers $y_i$, $lx_i$ and $rx_i$ ($0 &lt; y_i &lt; 10^6$; $0 \le lx_i &lt; rx_i \le 10^6$), which means the segment connects $(lx_i, y_i)$ and $(rx_i, y_i)$.</p><p>The next $m$ lines contain descriptions of the vertical segments. The $i$-th line contains three integers $x_i$, $ly_i$ and $ry_i$ ($0 &lt; x_i &lt; 10^6$; $0 \le ly_i &lt; ry_i \le 10^6$), which means the segment connects $(x_i, ly_i)$ and $(x_i, ry_i)$.</p><p>It's guaranteed that <span class="tex-font-style-bf">there are no two segments on the same line</span>, and each segment intersects with at least one of square's sides.</p></div><div class="output-specification"><p>Print the number of pieces the square is divided into after drawing all the segments.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($0 \le n, m \le 10^5$)&nbsp;— the number of horizontal segments and the number of vertical segments.</p><p>The next $n$ lines contain descriptions of the horizontal segments. The $i$-th line contains three integers $y_i$, $lx_i$ and $rx_i$ ($0 &lt; y_i &lt; 10^6$; $0 \le lx_i &lt; rx_i \le 10^6$), which means the segment connects $(lx_i, y_i)$ and $(rx_i, y_i)$.</p><p>The next $m$ lines contain descriptions of the vertical segments. The $i$-th line contains three integers $x_i$, $ly_i$ and $ry_i$ ($0 &lt; x_i &lt; 10^6$; $0 \le ly_i &lt; ry_i \le 10^6$), which means the segment connects $(x_i, ly_i)$ and $(x_i, ry_i)$.</p><p>It's guaranteed that <span class="tex-font-style-bf">there are no two segments on the same line</span>, and each segment intersects with at least one of square's sides.</p>

## Output

<p>Print the number of pieces the square is divided into after drawing all the segments.</p>





```input1
3 3
2 3 1000000
4 0 4
3 0 1000000
4 0 1
2 0 5
3 1 1000000
```




```output1
7
```



## Note

<p> The sample is like this:</p><center> <img class="tex-graphics" src="file://qtkhLdI7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
