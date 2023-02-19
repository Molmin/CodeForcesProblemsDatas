## Description

<div><p>There is a conveyor with $120$ rows and $120$ columns. Each row and column is numbered from $0$ to $119$, and the cell in $i$-th row and $j$-th column is denoted as $(i, j)$. The top leftmost cell is $(0, 0)$. Each cell has a belt, and all belts are initially facing to the right.</p><p>Initially, a slime ball is on the belt of $(0, 0)$, and other belts are empty. Every second, the state of the conveyor changes as follows: </p><ul> <li> All slime balls on the conveyor move one cell in the direction of the belt at the same time. If there is no cell in the moved position, the slime gets out of the conveyor, and if two slime balls move to the same cell, they merge into one. </li><li> All belts with slime ball in the previous second change direction at the same time: belts facing to the right become facing to the down, and vice versa. </li><li> A new slime ball is placed on cell $(0, 0)$. </li></ul><p>There are $q$ queries, each being three integers $t$, $x$, and $y$. You have to find out if there is a slime at the cell $(x, y)$ after $t$ seconds from the start. Can you do it?</p></div><div class="input-specification"><p>The first line contains one integer $q$ ($1 \le q \le 10^4$) — the number of queries.</p><p>The only line of each query contains three integers $t$, $x$, and $y$ ($0 \le t \le 10^{18}$, $0 \le x, y &lt; 120$).</p></div><div class="output-specification"><p>Print the answer for each test case, one per line. If there is a slime ball in the cell $(x, y)$ after $t$ seconds from the initial state, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains one integer $q$ ($1 \le q \le 10^4$) — the number of queries.</p><p>The only line of each query contains three integers $t$, $x$, and $y$ ($0 \le t \le 10^{18}$, $0 \le x, y &lt; 120$).</p>

## Output

<p>Print the answer for each test case, one per line. If there is a slime ball in the cell $(x, y)$ after $t$ seconds from the initial state, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1|2,4,6
6
1 1 0
5 1 3
0 0 0
2 4 5
2 0 2
1547748756 100 111
```




```output1
NO
YES
YES
NO
YES
YES
```



## Note

<p>The state of conveyor with $t = 0$. Red arrow represents the direction of each belt, and blue figure represents slime.</p><p><img class="tex-graphics" src="file://obTZt3ky.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The state of conveyor with $t = 1$.</p><p><img class="tex-graphics" src="file://ghw6ENtn.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The state of conveyor with $t = 2$.</p><p><img class="tex-graphics" src="file://128IHWAc.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
