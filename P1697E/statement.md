## Description

<div><p>You are given $n$ points on the plane, the coordinates of the $i$-th point are $(x_i, y_i)$. No two points have the same coordinates.</p><p>The distance between points $i$ and $j$ is defined as $d(i,j) = |x_i - x_j| + |y_i - y_j|$.</p><p>For each point, you have to choose a color, represented by an integer from $1$ to $n$. For every ordered triple of different points $(a,b,c)$, the following constraints should be met:</p><ul> <li> if $a$, $b$ and $c$ have the same color, then $d(a,b) = d(a,c) = d(b,c)$; </li><li> if $a$ and $b$ have the same color, and the color of $c$ is different from the color of $a$, then $d(a,b) &lt; d(a,c)$ and $d(a,b) &lt; d(b,c)$. </li></ul><p>Calculate the number of different ways to choose the colors that meet these constraints.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 100$)&nbsp;— the number of points.</p><p>Then $n$ lines follow. The $i$-th of them contains two integers $x_i$ and $y_i$ ($0 \le x_i, y_i \le 10^8$).</p><p>No two points have the same coordinates (i. e. if $i \ne j$, then either $x_i \ne x_j$ or $y_i \ne y_j$).</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of ways to choose the colors for the points. Since it can be large, print it modulo $998244353$.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 100$)&nbsp;— the number of points.</p><p>Then $n$ lines follow. The $i$-th of them contains two integers $x_i$ and $y_i$ ($0 \le x_i, y_i \le 10^8$).</p><p>No two points have the same coordinates (i. e. if $i \ne j$, then either $x_i \ne x_j$ or $y_i \ne y_j$).</p>

## Output

<p>Print one integer&nbsp;— the number of ways to choose the colors for the points. Since it can be large, print it modulo $998244353$.</p>





```input1
3
1 0
3 0
2 1
```




```input2
5
1 2
2 4
3 4
4 4
1 3
```




```input3
4
1 0
3 0
2 1
2 0
```




```output1
9
```




```output2
240
```




```output3
24
```



## Note

<p>In the first test, the following ways to choose the colors are suitable:</p><ul> <li> $[1, 1, 1]$; </li><li> $[2, 2, 2]$; </li><li> $[3, 3, 3]$; </li><li> $[1, 2, 3]$; </li><li> $[1, 3, 2]$; </li><li> $[2, 1, 3]$; </li><li> $[2, 3, 1]$; </li><li> $[3, 1, 2]$; </li><li> $[3, 2, 1]$. </li></ul>
