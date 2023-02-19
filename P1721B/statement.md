## Description

<div><p>The robot is placed in the top left corner of a grid, consisting of $n$ rows and $m$ columns, in a cell $(1, 1)$.</p><p>In one step, it can move into a cell, adjacent by a side to the current one: </p><ul> <li> $(x, y) \rightarrow (x, y + 1)$; </li><li> $(x, y) \rightarrow (x + 1, y)$; </li><li> $(x, y) \rightarrow (x, y - 1)$; </li><li> $(x, y) \rightarrow (x - 1, y)$. </li></ul><p>The robot can't move outside the grid.</p><p>The cell $(s_x, s_y)$ contains a deadly laser. If the robot comes into some cell that has distance less than or equal to $d$ to the laser, it gets evaporated. The distance between two cells $(x_1, y_1)$ and $(x_2, y_2)$ is $|x_1 - x_2| + |y_1 - y_2|$.</p><p>Print the smallest number of steps that the robot can take to reach the cell $(n, m)$ without getting evaporated or moving outside the grid. If it's not possible to reach the cell $(n, m)$, print <span class="tex-font-style-tt">-1</span>.</p><p>The laser is neither in the starting cell, nor in the ending cell. The starting cell always has distance greater than $d$ to the laser.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains five integers $n, m, s_x, s_y, d$ ($2 \le n, m \le 1000$; $1 \le s_x \le n$; $1 \le s_y \le m$; $0 \le d \le n + m$)&nbsp;— the size of the grid, the cell that contains the laser and the evaporating distance of the laser.</p><p>The laser is neither in the starting cell, nor in the ending cell ($(s_x, s_y) \neq (1, 1)$ and $(s_x, s_y) \neq (n, m)$). The starting cell $(1, 1)$ always has distance greater than $d$ to the laser ($|s_x - 1| + |s_y - 1| &gt; d$).</p></div><div class="output-specification"><p>For each testcase, print a single integer. If it's possible to reach the cell $(n, m)$ from $(1, 1)$ without getting evaporated or moving outside the grid, then print the smallest amount of steps it can take the robot to reach it. Otherwise, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains five integers $n, m, s_x, s_y, d$ ($2 \le n, m \le 1000$; $1 \le s_x \le n$; $1 \le s_y \le m$; $0 \le d \le n + m$)&nbsp;— the size of the grid, the cell that contains the laser and the evaporating distance of the laser.</p><p>The laser is neither in the starting cell, nor in the ending cell ($(s_x, s_y) \neq (1, 1)$ and $(s_x, s_y) \neq (n, m)$). The starting cell $(1, 1)$ always has distance greater than $d$ to the laser ($|s_x - 1| + |s_y - 1| &gt; d$).</p>

## Output

<p>For each testcase, print a single integer. If it's possible to reach the cell $(n, m)$ from $(1, 1)$ without getting evaporated or moving outside the grid, then print the smallest amount of steps it can take the robot to reach it. Otherwise, print <span class="tex-font-style-tt">-1</span>.</p>





```input1|2,4
3
2 3 1 3 0
2 3 1 3 1
5 5 3 4 1
```




```output1
3
-1
8
```


