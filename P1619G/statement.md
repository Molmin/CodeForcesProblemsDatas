## Description

<div><p>Polycarp is very fond of playing the game Minesweeper. Recently he found a similar game and there are such rules.</p><p>There are mines on the field, for each the coordinates of its location are known ($x_i, y_i$). Each mine has a lifetime in seconds, after which it will explode. After the explosion, the mine also detonates all mines vertically and horizontally at a distance of $k$ (two perpendicular lines). As a result, we get an explosion on the field in the form of a "plus" symbol ('<span class="tex-font-style-bf">+</span>'). Thus, one explosion can cause new explosions, and so on.</p><p>Also, Polycarp can detonate anyone mine every second, starting from zero seconds. After that, a chain reaction of explosions also takes place. Mines explode <span class="tex-font-style-bf">instantly</span> and also <span class="tex-font-style-bf">instantly</span> detonate other mines according to the rules described above.</p><p>Polycarp wants to set a new record and asks you to help him calculate in what minimum number of seconds all mines can be detonated.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>An empty line is written in front of each test suite.</p><p>Next comes a line that contains integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $0 \le k \le 10^9$) — the number of mines and the distance that hit by mines during the explosion, respectively.</p><p>Then $n$ lines follow, the $i$-th of which describes the $x$ and $y$ coordinates of the $i$-th mine and the time until its explosion ($-10^9 \le x, y \le 10^9$, $0 \le timer \le 10^9$). It is guaranteed that all mines have different coordinates.</p><p>It is guaranteed that the sum of the values $n$ over all test cases in the test does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $t$ lines, each of the lines must contain the answer to the corresponding set of input data &nbsp;— the minimum number of seconds it takes to explode all the mines.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test.</p><p>An empty line is written in front of each test suite.</p><p>Next comes a line that contains integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $0 \le k \le 10^9$) — the number of mines and the distance that hit by mines during the explosion, respectively.</p><p>Then $n$ lines follow, the $i$-th of which describes the $x$ and $y$ coordinates of the $i$-th mine and the time until its explosion ($-10^9 \le x, y \le 10^9$, $0 \le timer \le 10^9$). It is guaranteed that all mines have different coordinates.</p><p>It is guaranteed that the sum of the values $n$ over all test cases in the test does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Print $t$ lines, each of the lines must contain the answer to the corresponding set of input data &nbsp;— the minimum number of seconds it takes to explode all the mines.</p>





```input1
3

5 0
0 0 1
0 1 4
1 0 2
1 1 3
2 2 9

5 2
0 0 1
0 1 4
1 0 2
1 1 3
2 2 9

6 1
1 -1 3
0 -1 9
0 1 7
-1 0 1
-1 1 9
-1 -1 7
```




```output1
2
1
0
```



## Note

<center> <img class="tex-graphics" src="file://CEbGbDgp.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px">   <span class="tex-font-size-small">Picture from examples</span> </center><p>First example: </p><ul><li> $0$ second: we explode a mine at the cell $(2, 2)$, it does not detonate any other mine since $k=0$. </li><li> $1$ second: we explode the mine at the cell $(0, 1)$, and the mine at the cell $(0, 0)$ explodes itself. </li><li> $2$ second: we explode the mine at the cell $(1, 1)$, and the mine at the cell $(1, 0)$ explodes itself.</li></ul><p>Second example:</p><ul> <li> $0$ second: we explode a mine at the cell $(2, 2)$ we get: </li></ul><center> <img class="tex-graphics" src="file://CVmJDenu.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px">   </center><ul> <li> $1$ second: the mine at coordinate $(0, 0)$ explodes and since $k=2$ the explosion detonates mines at the cells $(0, 1)$ and $(1, 0)$, and their explosions detonate the mine at the cell $(1, 1)$ and there are no mines left on the field. </li></ul>
