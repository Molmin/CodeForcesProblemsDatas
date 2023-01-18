## Description

<div><p>A <span class="tex-font-style-it">star</span> is a figure of the following type: an asterisk character '<span class="tex-font-style-tt">*</span>' in the center of the figure and four rays (to the left, right, top, bottom) of the same positive length. The size of a <span class="tex-font-style-it">star</span> is the length of its rays. The size of a star must be a positive number (i.e. rays of length $0$ are not allowed).</p><p>Let's consider empty cells are denoted by '<span class="tex-font-style-tt">.</span>', then the following figures are <span class="tex-font-style-it">stars</span>:</p><center> <img class="tex-graphics" src="file://8biCtzB4.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The leftmost figure is a <span class="tex-font-style-it">star</span> of size $1$, the middle figure is a <span class="tex-font-style-it">star</span> of size $2$ and the rightmost figure is a <span class="tex-font-style-it">star</span> of size $3$.</span> </center><p>You are given a rectangular grid of size $n \times m$ consisting only of asterisks '<span class="tex-font-style-tt">*</span>' and periods (dots) '<span class="tex-font-style-tt">.</span>'. Rows are numbered from $1$ to $n$, columns are numbered from $1$ to $m$. Your task is to draw this grid using <span class="tex-font-style-it">any</span> number of <span class="tex-font-style-it">stars</span> or find out that it is impossible. <span class="tex-font-style-it">Stars</span> can intersect, overlap or even coincide with each other. The number of <span class="tex-font-style-it">stars</span> in the output can't exceed $n \cdot m$. Each star should be completely inside the grid. You can use stars of same and arbitrary sizes.</p><p><span class="tex-font-style-it">In this problem, you do not need to minimize the number of stars. Just find any way to draw the given grid with at most $n \cdot m$ stars.</span></p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $m$ ($3 \le n, m \le 100$) — the sizes of the given grid.</p><p>The next $n$ lines contains $m$ characters each, the $i$-th line describes the $i$-th row of the grid. It is guaranteed that grid consists of characters '<span class="tex-font-style-tt">*</span>' and '<span class="tex-font-style-tt">.</span>' only.</p></div><div class="output-specification"><p>If it is impossible to draw the given grid using <span class="tex-font-style-it">stars</span> only, print "<span class="tex-font-style-tt">-1</span>".</p><p>Otherwise in the first line print one integer $k$ ($0 \le k \le n \cdot m$) — the number of <span class="tex-font-style-it">stars</span> needed to draw the given grid. The next $k$ lines should contain three integers each — $x_j$, $y_j$ and $s_j$, where $x_j$ is the row index of the central <span class="tex-font-style-it">star</span> character, $y_j$ is the column index of the central <span class="tex-font-style-it">star</span> character and $s_j$ is the size of the <span class="tex-font-style-it">star</span>. Each <span class="tex-font-style-it">star</span> should be completely inside the grid.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $m$ ($3 \le n, m \le 100$) — the sizes of the given grid.</p><p>The next $n$ lines contains $m$ characters each, the $i$-th line describes the $i$-th row of the grid. It is guaranteed that grid consists of characters '<span class="tex-font-style-tt">*</span>' and '<span class="tex-font-style-tt">.</span>' only.</p>

## Output

<p>If it is impossible to draw the given grid using <span class="tex-font-style-it">stars</span> only, print "<span class="tex-font-style-tt">-1</span>".</p><p>Otherwise in the first line print one integer $k$ ($0 \le k \le n \cdot m$) — the number of <span class="tex-font-style-it">stars</span> needed to draw the given grid. The next $k$ lines should contain three integers each — $x_j$, $y_j$ and $s_j$, where $x_j$ is the row index of the central <span class="tex-font-style-it">star</span> character, $y_j$ is the column index of the central <span class="tex-font-style-it">star</span> character and $s_j$ is the size of the <span class="tex-font-style-it">star</span>. Each <span class="tex-font-style-it">star</span> should be completely inside the grid.</p>





```input1
6 8
....*...
...**...
..*****.
...**...
....*...
........

```




```input2
5 5
.*...
****.
.****
..**.
.....

```




```input3
5 5
.*...
***..
.*...
.*...
.....

```




```input4
3 3
*.*
.*.
*.*

```




```output1
3
3 4 1
3 5 2
3 5 1

```




```output2
3
2 2 1
3 3 1
3 4 1

```




```output3
-1

```




```output4
-1

```



## Note

<p>In the first example the output </p><pre class="verbatim">2<br>3 4 1<br>3 5 2<br></pre><p>is also correct.</p>
