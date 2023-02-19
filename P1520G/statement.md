## Description

<div><p>Dima overslept the alarm clock, which was supposed to raise him to school.</p><p>Dima wonders if he will have time to come to the first lesson. To do this, he needs to know the <span class="tex-font-style-bf">minimum time</span> it will take him to get from home to school.</p><p>The city where Dima lives is a rectangular field of $n \times m$ size. Each cell $(i, j)$ on this field is denoted by one number $a_{ij}$:</p><ul> <li> The number $-1$ means that the passage through the cell is prohibited; </li><li> The number $0$ means that the cell is free and Dima can walk though it. </li><li> The number $x$ ($1 \le x \le 10^9$) means that the cell contains a portal with a cost of $x$. A cell with a portal is also considered free. </li></ul><p>From any portal, Dima can go to any other portal, while the time of moving from the portal $(i, j)$ to the portal $(x, y)$ corresponds to the sum of their costs $a_{ij} + a_{xy}$.</p><p>In addition to moving between portals, Dima can also move between unoccupied cells adjacent to one side in time $w$. In particular, he can enter a cell with a portal and not use it.</p><p>Initially, Dima is in the upper-left cell $(1, 1)$, and the school is in the lower right cell $(n, m)$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $w$ ($2 \le n, m \le 2 \cdot 10^3$, $1 \le w \le 10^9$), where $n$ and $m$ are city size, $w$ is time during which Dima moves between unoccupied cells.</p><p>The next $n$ lines each contain $m$ numbers ($-1 \le a_{ij} \le 10^9$)&nbsp;— descriptions of cells.</p><p>It is guaranteed that the cells $(1, 1)$ and $(n, m)$ are free.</p></div><div class="output-specification"><p>Output the minimum time it will take for Dima to get to school. If he cannot get to school at all, then output "<span class="tex-font-style-tt">-1</span>".</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $w$ ($2 \le n, m \le 2 \cdot 10^3$, $1 \le w \le 10^9$), where $n$ and $m$ are city size, $w$ is time during which Dima moves between unoccupied cells.</p><p>The next $n$ lines each contain $m$ numbers ($-1 \le a_{ij} \le 10^9$)&nbsp;— descriptions of cells.</p><p>It is guaranteed that the cells $(1, 1)$ and $(n, m)$ are free.</p>

## Output

<p>Output the minimum time it will take for Dima to get to school. If he cannot get to school at all, then output "<span class="tex-font-style-tt">-1</span>".</p>





```input1
5 5 1
0 -1 0 1 -1
0 20 0 0 -1
-1 -1 -1 -1 -1
3 0 0 0 0
-1 0 0 0 0
```




```output1
14
```



## Note

<p>Explanation for the first sample: </p><center> <img class="tex-graphics" src="file://XMdjxNCS.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
