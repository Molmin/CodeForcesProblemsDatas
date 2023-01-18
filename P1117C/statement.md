## Description

<div><p>You a captain of a ship. Initially you are standing in a point $(x_1, y_1)$ (obviously, all positions in the sea can be described by cartesian plane) and you want to travel to a point $(x_2, y_2)$. </p><p>You know the weather forecast — the string $s$ of length $n$, consisting only of letters <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">L</span> and <span class="tex-font-style-tt">R</span>. The letter corresponds to a direction of wind. Moreover, the forecast is periodic, e.g. the first day wind blows to the side $s_1$, the second day — $s_2$, the $n$-th day — $s_n$ and $(n+1)$-th day — $s_1$ again and so on. </p><p>Ship coordinates change the following way:</p><ul> <li> if wind blows the direction <span class="tex-font-style-tt">U</span>, then the ship moves from $(x, y)$ to $(x, y + 1)$; </li><li> if wind blows the direction <span class="tex-font-style-tt">D</span>, then the ship moves from $(x, y)$ to $(x, y - 1)$; </li><li> if wind blows the direction <span class="tex-font-style-tt">L</span>, then the ship moves from $(x, y)$ to $(x - 1, y)$; </li><li> if wind blows the direction <span class="tex-font-style-tt">R</span>, then the ship moves from $(x, y)$ to $(x + 1, y)$. </li></ul><p>The ship can also either go one of the four directions or stay in place each day. If it goes then it's exactly 1 unit of distance. Transpositions of the ship and the wind add up. If the ship stays in place, then only the direction of wind counts. For example, if wind blows the direction <span class="tex-font-style-tt">U</span> and the ship moves the direction <span class="tex-font-style-tt">L</span>, then from point $(x, y)$ it will move to the point $(x - 1, y + 1)$, and if it goes the direction <span class="tex-font-style-tt">U</span>, then it will move to the point $(x, y + 2)$.</p><p>You task is to determine the minimal number of days required for the ship to reach the point $(x_2, y_2)$.</p></div><div class="input-specification"><p>The first line contains two integers $x_1, y_1$ ($0 \le x_1, y_1 \le 10^9$) — the initial coordinates of the ship.</p><p>The second line contains two integers $x_2, y_2$ ($0 \le x_2, y_2 \le 10^9$) — the coordinates of the destination point.</p><p>It is guaranteed that the initial coordinates and destination point coordinates are different.</p><p>The third line contains a single integer $n$ ($1 \le n \le 10^5$) — the length of the string $s$.</p><p>The fourth line contains the string $s$ itself, consisting only of letters <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">L</span> and <span class="tex-font-style-tt">R</span>.</p></div><div class="output-specification"><p>The only line should contain the minimal number of days required for the ship to reach the point $(x_2, y_2)$.</p><p>If it's impossible then print "<span class="tex-font-style-tt">-1</span>".</p></div>

## Input

<p>The first line contains two integers $x_1, y_1$ ($0 \le x_1, y_1 \le 10^9$) — the initial coordinates of the ship.</p><p>The second line contains two integers $x_2, y_2$ ($0 \le x_2, y_2 \le 10^9$) — the coordinates of the destination point.</p><p>It is guaranteed that the initial coordinates and destination point coordinates are different.</p><p>The third line contains a single integer $n$ ($1 \le n \le 10^5$) — the length of the string $s$.</p><p>The fourth line contains the string $s$ itself, consisting only of letters <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">L</span> and <span class="tex-font-style-tt">R</span>.</p>

## Output

<p>The only line should contain the minimal number of days required for the ship to reach the point $(x_2, y_2)$.</p><p>If it's impossible then print "<span class="tex-font-style-tt">-1</span>".</p>





```input1
0 0
4 6
3
UUU
```




```input2
0 3
0 0
3
UDD
```




```input3
0 0
0 1
1
L
```




```output1
5
```




```output2
3
```




```output3
-1
```



## Note

<p>In the first example the ship should perform the following sequence of moves: "<span class="tex-font-style-tt">RRRRU</span>". Then its coordinates will change accordingly: $(0, 0)$ $\rightarrow$ $(1, 1)$ $\rightarrow$ $(2, 2)$ $\rightarrow$ $(3, 3)$ $\rightarrow$ $(4, 4)$ $\rightarrow$ $(4, 6)$.</p><p>In the second example the ship should perform the following sequence of moves: "<span class="tex-font-style-tt">DD</span>" (the third day it should stay in place). Then its coordinates will change accordingly: $(0, 3)$ $\rightarrow$ $(0, 3)$ $\rightarrow$ $(0, 1)$ $\rightarrow$ $(0, 0)$.</p><p>In the third example the ship can never reach the point $(0, 1)$.</p>
