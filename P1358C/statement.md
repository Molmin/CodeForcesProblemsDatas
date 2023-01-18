## Description

<div><p>During the quarantine, Sicromoft has more free time to create the new functions in "<span class="tex-font-style-tt">Celex-2021</span>". The developers made a new function <span class="tex-font-style-tt">GAZ-GIZ</span>, which infinitely fills an infinite table to the right and down from the upper left corner as follows:</p><center> <img class="tex-graphics" src="file://5FxEpps5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> The cell with coordinates $(x, y)$ is at the intersection of $x$-th row and $y$-th column. Upper left cell $(1,1)$ contains an integer $1$.<p>The developers of the <span class="tex-font-style-tt">SUM</span> function don't sleep either. Because of the boredom, they teamed up with the developers of the <span class="tex-font-style-tt">RAND</span> function, so they added the ability to calculate the sum on an arbitrary path from one cell to another, moving down or right. Formally, from the cell $(x,y)$ in one step you can move to the cell $(x+1, y)$ or $(x, y+1)$. </p><p>After another Dinwows update, Levian started to study "<span class="tex-font-style-tt">Celex-2021</span>" (because he wants to be an accountant!). After filling in the table with the <span class="tex-font-style-tt">GAZ-GIZ</span> function, he asked you to calculate the quantity of possible different amounts on the path from a given cell $(x_1, y_1)$ to another given cell $(x_2, y_2$), if you can only move one cell down or right.</p><p>Formally, consider all the paths from the cell $(x_1, y_1)$ to cell $(x_2, y_2)$ such that each next cell in the path is located either to the down or to the right of the previous one. Calculate the number of different sums of elements for all such paths.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 57179$) — the number of test cases.</p><p>Each of the following $t$ lines contains four natural numbers $x_1$, $y_1$, $x_2$, $y_2$ ($1 \le x_1 \le x_2 \le 10^9$, $1 \le y_1 \le y_2 \le 10^9$) — coordinates of the start and the end cells. </p></div><div class="output-specification"><p>For each test case, in a separate line, print the number of possible different sums on the way from the start cell to the end cell.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 57179$) — the number of test cases.</p><p>Each of the following $t$ lines contains four natural numbers $x_1$, $y_1$, $x_2$, $y_2$ ($1 \le x_1 \le x_2 \le 10^9$, $1 \le y_1 \le y_2 \le 10^9$) — coordinates of the start and the end cells. </p>

## Output

<p>For each test case, in a separate line, print the number of possible different sums on the way from the start cell to the end cell.</p>





```input1
4
1 1 2 2
1 2 2 4
179 1 179 100000
5 7 5 7
```




```output1
2
3
1
1
```



## Note

<p>In the first test case there are two possible sums: $1+2+5=8$ and $1+3+5=9$. <img class="tex-graphics" src="file://nx45heHH.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
