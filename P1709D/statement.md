## Description

<div><p>There is a grid, consisting of $n$ rows and $m$ columns. The rows are numbered from $1$ to $n$ from bottom to top. The columns are numbered from $1$ to $m$ from left to right. The $i$-th column has the bottom $a_i$ cells blocked (the cells in rows $1, 2, \dots, a_i$), the remaining $n - a_i$ cells are unblocked.</p><p>A robot is travelling across this grid. You can send it commands&nbsp;— move up, right, down or left. If a robot attempts to move into a blocked cell or outside the grid, it explodes.</p><p>However, the robot is broken&nbsp;— it executes each received command $k$ times. So if you tell it to move up, for example, it will move up $k$ times ($k$ cells). You can't send it commands while the robot executes the current one.</p><p>You are asked $q$ queries about the robot. Each query has a start cell, a finish cell and a value $k$. Can you send the robot an arbitrary number of commands (possibly, zero) so that it reaches the finish cell from the start cell, given that it executes each command $k$ times?</p><p>The robot must stop in the finish cell. If it visits the finish cell while still executing commands, it doesn't count.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^9$; $1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of rows and columns of the grid.</p><p>The second line contains $m$ integers $a_1, a_2, \dots, a_m$ ($0 \le a_i \le n$)&nbsp;— the number of blocked cells on the bottom of the $i$-th column.</p><p>The third line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contain five integers $x_s, y_s, x_f, y_f$ and $k$ ($a[y_s] &lt; x_s \le n$; $1 \le y_s \le m$; $a[y_f] &lt; x_f \le n$; $1 \le y_f \le m$; $1 \le k \le 10^9$)&nbsp;— the row and the column of the start cell, the row and the column of the finish cell and the number of times each your command is executed. The start and the finish cell of each query are unblocked.</p></div><div class="output-specification"><p>For each query, print "<span class="tex-font-style-tt">YES</span>" if you can send the robot an arbitrary number of commands (possibly, zero) so that it reaches the finish cell from the start cell, given that it executes each command $k$ times. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^9$; $1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of rows and columns of the grid.</p><p>The second line contains $m$ integers $a_1, a_2, \dots, a_m$ ($0 \le a_i \le n$)&nbsp;— the number of blocked cells on the bottom of the $i$-th column.</p><p>The third line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contain five integers $x_s, y_s, x_f, y_f$ and $k$ ($a[y_s] &lt; x_s \le n$; $1 \le y_s \le m$; $a[y_f] &lt; x_f \le n$; $1 \le y_f \le m$; $1 \le k \le 10^9$)&nbsp;— the row and the column of the start cell, the row and the column of the finish cell and the number of times each your command is executed. The start and the finish cell of each query are unblocked.</p>

## Output

<p>For each query, print "<span class="tex-font-style-tt">YES</span>" if you can send the robot an arbitrary number of commands (possibly, zero) so that it reaches the finish cell from the start cell, given that it executes each command $k$ times. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
11 10
9 0 0 10 3 4 8 11 10 8
6
1 2 1 3 1
1 2 1 3 2
4 3 4 5 2
5 3 11 5 3
5 3 11 5 2
11 9 9 10 1
```




```output1
YES
NO
NO
NO
YES
YES
```


