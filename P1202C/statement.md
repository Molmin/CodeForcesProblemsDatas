## Description

<div><p>You have a string $s$ — a sequence of commands for your toy robot. The robot is placed in some cell of a <span class="tex-font-style-bf">rectangular</span> grid. He can perform four commands:</p><ul> <li> 'W' — move one cell up; </li><li> 'S' — move one cell down; </li><li> 'A' — move one cell left; </li><li> 'D' — move one cell right. </li></ul><p>Let $Grid(s)$ be the grid of minimum possible area such that there is a position in the grid where you can place the robot in such a way that it will not fall from the grid while running the sequence of commands $s$. For example, if $s = \text{DSAWWAW}$ then $Grid(s)$ is the $4 \times 3$ grid:</p><ol> <li> you can place the robot in the cell $(3, 2)$; </li><li> the robot performs the command 'D' and moves to $(3, 3)$; </li><li> the robot performs the command 'S' and moves to $(4, 3)$; </li><li> the robot performs the command 'A' and moves to $(4, 2)$; </li><li> the robot performs the command 'W' and moves to $(3, 2)$; </li><li> the robot performs the command 'W' and moves to $(2, 2)$; </li><li> the robot performs the command 'A' and moves to $(2, 1)$; </li><li> the robot performs the command 'W' and moves to $(1, 1)$. </li></ol><center> <img class="tex-graphics" src="file://1ca47YjU.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You have $4$ extra letters: one 'W', one 'A', one 'S', one 'D'. You'd like to insert <span class="tex-font-style-bf">at most one of these letters</span> in any position of sequence $s$ to minimize the area of $Grid(s)$.</p><p>What is the minimum area of $Grid(s)$ you can achieve?</p></div><div class="input-specification"><p>The first line contains one integer $T$ ($1 \le T \le 1000$) — the number of queries.</p><p>Next $T$ lines contain queries: one per line. This line contains single string $s$ ($1 \le |s| \le 2 \cdot 10^5$, $s_i \in \{\text{W}, \text{A}, \text{S}, \text{D}\}$) — the sequence of commands.</p><p>It's guaranteed that the total length of $s$ over all queries doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $T$ integers: one per query. For each query print the minimum area of $Grid(s)$ you can achieve.</p></div>

## Input

<p>The first line contains one integer $T$ ($1 \le T \le 1000$) — the number of queries.</p><p>Next $T$ lines contain queries: one per line. This line contains single string $s$ ($1 \le |s| \le 2 \cdot 10^5$, $s_i \in \{\text{W}, \text{A}, \text{S}, \text{D}\}$) — the sequence of commands.</p><p>It's guaranteed that the total length of $s$ over all queries doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>Print $T$ integers: one per query. For each query print the minimum area of $Grid(s)$ you can achieve.</p>





```input1
3
DSAWWAW
D
WA
```




```output1
8
2
4
```



## Note

<p>In the first query you have to get string $\text{DSAWW}\underline{D}\text{AW}$.</p><p>In second and third queries you can not decrease the area of $Grid(s)$.</p>
