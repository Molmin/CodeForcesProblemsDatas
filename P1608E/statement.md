## Description

<div><p>On an endless checkered sheet of paper, $n$ cells are chosen and colored in three colors, where $n$ is divisible by $3$. It turns out that there are exactly $\frac{n}{3}$ marked cells of each of three colors! </p><p>Find the largest such $k$ that it's possible to choose $\frac{k}{3}$ cells of each color, remove all other marked cells, and then select three rectangles with sides parallel to the grid lines so that the following conditions hold:</p><ul> <li> No two rectangles can intersect (but they can share a part of the boundary). In other words, the area of intersection of any two of these rectangles must be $0$.</li><li> The $i$-th rectangle contains all the chosen cells of the $i$-th color and no chosen cells of other colors, for $i = 1, 2, 3$. </li></ul></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ — the number of the marked cells ($3 \leq n \le 10^5$, $n$ is divisible by 3).</p><p>The $i$-th of the following $n$ lines contains three integers $x_i$, $y_i$, $c_i$ ($|x_i|,|y_i| \leq 10^9$; $1 \leq c_i \leq 3$), where $(x_i, y_i)$ are the coordinates of the $i$-th marked cell and $c_i$ is its color.</p><p>It's guaranteed that all cells $(x_i, y_i)$ in the input are distinct, and that there are exactly $\frac{n}{3}$ cells of each color.</p></div><div class="output-specification"><p>Output a single integer $k$ — the largest number of cells you can leave.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ — the number of the marked cells ($3 \leq n \le 10^5$, $n$ is divisible by 3).</p><p>The $i$-th of the following $n$ lines contains three integers $x_i$, $y_i$, $c_i$ ($|x_i|,|y_i| \leq 10^9$; $1 \leq c_i \leq 3$), where $(x_i, y_i)$ are the coordinates of the $i$-th marked cell and $c_i$ is its color.</p><p>It's guaranteed that all cells $(x_i, y_i)$ in the input are distinct, and that there are exactly $\frac{n}{3}$ cells of each color.</p>

## Output

<p>Output a single integer $k$ — the largest number of cells you can leave.</p>





```input1
9
2 3 1
4 1 2
2 1 3
3 4 1
5 3 2
4 4 3
2 4 1
5 2 2
3 5 3
```




```input2
3
1 1 1
2 2 2
3 3 3
```




```output1
6
```




```output2
3
```



## Note

<p>In the first sample, it's possible to leave $6$ cells with indexes $1, 5, 6, 7, 8, 9$.</p><p>In the second sample, it's possible to leave $3$ cells with indexes $1, 2, 3$.</p>
