## Description

<div><p>There is a square grid of size $n \times n$. Some cells are colored in black, all others are colored in white. In one operation you can select some rectangle and color all its cells in white. It costs $\max(h, w)$ to color a rectangle of size $h \times w$. You are to make all cells white for minimum total cost.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 50$)&nbsp;— the size of the square grid.</p><p>Each of the next $n$ lines contains a string of length $n$, consisting of characters '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">#</span>'. The $j$-th character of the $i$-th line is '<span class="tex-font-style-tt">#</span>' if the cell with coordinates $(i, j)$ is black, otherwise it is white.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum total cost to paint all cells in white.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 50$)&nbsp;— the size of the square grid.</p><p>Each of the next $n$ lines contains a string of length $n$, consisting of characters '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">#</span>'. The $j$-th character of the $i$-th line is '<span class="tex-font-style-tt">#</span>' if the cell with coordinates $(i, j)$ is black, otherwise it is white.</p>

## Output

<p>Print a single integer&nbsp;— the minimum total cost to paint all cells in white.</p>





```input1
3
###
#.#
###
```




```input2
3
...
...
...
```




```input3
4
#...
....
....
#...
```




```input4
5
#...#
.#.#.
.....
.#...
#....
```




```output1
3
```




```output2
0
```




```output3
2
```




```output4
5
```



## Note

<p>The examples and some of optimal solutions are shown on the pictures below.</p><center> <img class="tex-graphics" src="file://Gos3Jrj7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
