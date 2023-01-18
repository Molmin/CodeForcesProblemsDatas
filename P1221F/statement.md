## Description

<div><p>Petya recently found a game "Choose a Square". In this game, there are $n$ points numbered from $1$ to $n$ on an infinite field. The $i$-th point has coordinates $(x_i, y_i)$ and cost $c_i$.</p><p>You have to choose a square such that its sides are parallel to coordinate axes, the lower left and upper right corners belong to the line $y = x$, and all corners have integer coordinates.</p><p>The score you get is the sum of costs of the points covered by the selected square minus the length of the side of the square. Note that the length of the side can be zero.</p><p>Petya asks you to calculate the maximum possible score in the game that can be achieved by placing exactly one square.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the number of points on the field.</p><p>Each of the following $n$ lines contains three integers $x_i, y_i, c_i$ ($0 \le x_i, y_i \le 10^9, -10^6 \le c_i \le 10^6$) — coordinates of the $i$-th point and its cost, respectively.</p></div><div class="output-specification"><p>In the first line print the maximum score Petya can achieve.</p><p>In the second line print four integers $x_1, y_1, x_2, y_2$ ($0 \le x_1, y_1, x_2, y_2 \le 2 \cdot 10^9, x_1 = y_1, x_2 = y_2, x_1 \le x_2$) separated by spaces — the coordinates of the lower left and upper right corners of the square which Petya has to select in order to achieve the maximum score.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the number of points on the field.</p><p>Each of the following $n$ lines contains three integers $x_i, y_i, c_i$ ($0 \le x_i, y_i \le 10^9, -10^6 \le c_i \le 10^6$) — coordinates of the $i$-th point and its cost, respectively.</p>

## Output

<p>In the first line print the maximum score Petya can achieve.</p><p>In the second line print four integers $x_1, y_1, x_2, y_2$ ($0 \le x_1, y_1, x_2, y_2 \le 2 \cdot 10^9, x_1 = y_1, x_2 = y_2, x_1 \le x_2$) separated by spaces — the coordinates of the lower left and upper right corners of the square which Petya has to select in order to achieve the maximum score.</p>





```input1
6
0 0 2
1 0 -5
1 1 3
2 3 4
1 4 -4
3 1 -1
```




```input2
5
3 3 0
3 3 -3
0 2 -1
3 1 3
0 0 -2
```




```output1
4
1 1 3 3
```




```output2
0
1 1 1 1
```



## Note

<p>The field corresponding to the first example: <img class="tex-graphics" src="file://yGxziJSW.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
