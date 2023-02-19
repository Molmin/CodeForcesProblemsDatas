## Description

<div><p>Polycarp has a rectangular field of $n \times m$ cells (the size of the $n \cdot m$ field does not exceed $10^6$ cells, $m \ge 2$), in each cell of which there can be candy. There are $n$ rows and $m$ columns in the field.</p><p>Let's denote a cell with coordinates $x$ vertically and $y$ horizontally by $(x, y)$. Then the top-left cell will be denoted as $(1, 1)$, and the bottom-right cell will be denoted as $(n, m)$.</p><p>If there is candy in the cell, then the cell is marked with the symbol '<span class="tex-font-style-tt">1</span>', otherwise&nbsp;— with the symbol '<span class="tex-font-style-tt">0</span>'.</p><p>Polycarp made a Robot that can collect candy. The Robot can move from $(x, y)$ either to $(x+1, y+1)$, or to $(x+1, y-1)$. If the Robot is in a cell that contains candy, it takes it.</p><p>While there is at least one candy on the field, the following procedure is executed: </p><ul> <li> Polycarp puts the Robot in an arbitrary cell on the <span class="tex-font-style-bf">topmost row</span> of the field. He himself chooses in which cell to place the Robot. It is allowed to put the Robot in the same cell multiple times. </li><li> The Robot moves across the field and collects candies. He controls the Robot. </li><li> When the Robot leaves the field, Polycarp takes it. If there are still candies left, Polycarp repeats the procedure. </li></ul><p>Find the <span class="tex-font-style-bf">minimum</span> number of times Polycarp needs to put the Robot on the topmost row of the field in order to collect all the candies. It is guaranteed that Polycarp can always collect all the candies.</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$) — the number of input data sets in the test.</p><p>Before each input data, there is a blank line in the test. Next is a line that contains integers $n$ and $m$ ($2 \le m$, $2 \le n \cdot m \le 10^6$) — field sizes. This is followed by $n$ lines, $i$-th of which describes the $i$-th line of the field. Each of them is a string of size $m$ characters: the symbol '<span class="tex-font-style-tt">1</span>' corresponds to a cell with candy, the symbol '<span class="tex-font-style-tt">0</span>'&nbsp;— an empty cell.</p><p>It is guaranteed that the sum of $n \cdot m$ values for all input data sets in the test does not exceed $10^6$.</p></div><div class="output-specification"><p>Print $t$ lines, each line should contain the answer to the corresponding set of input data: the minimum number of times Polycarpus needs to put the Robot on the topmost row of the field in order to collect all the candies.</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$) — the number of input data sets in the test.</p><p>Before each input data, there is a blank line in the test. Next is a line that contains integers $n$ and $m$ ($2 \le m$, $2 \le n \cdot m \le 10^6$) — field sizes. This is followed by $n$ lines, $i$-th of which describes the $i$-th line of the field. Each of them is a string of size $m$ characters: the symbol '<span class="tex-font-style-tt">1</span>' corresponds to a cell with candy, the symbol '<span class="tex-font-style-tt">0</span>'&nbsp;— an empty cell.</p><p>It is guaranteed that the sum of $n \cdot m$ values for all input data sets in the test does not exceed $10^6$.</p>

## Output

<p>Print $t$ lines, each line should contain the answer to the corresponding set of input data: the minimum number of times Polycarpus needs to put the Robot on the topmost row of the field in order to collect all the candies.</p>





```input1
4

2 2
00
00

3 3
100
000
101

4 5
01000
00001
00010
10000

3 3
111
111
111
```




```output1
0
2
2
4
```



## Note

<p>In the first set Polycarp may not put the Robot on the field at all, so the answer "<span class="tex-font-style-tt">0</span>"</p><p>In the second set, Polycarp will need to place the robot on the field twice. The Robot can collect candies like this: for the first time Polycarp puts the Robot in the cell $(1, 1)$ and collects candies at the positions $(1, 1)$ and $(3, 3)$. The second time Polycarp can again put the Robot in $(1, 1)$, and then the Robot will move first to $(2,2)$, then to $(3, 1)$ and collect the last candy.</p><p>In the fourth set, you can show that the Robot cannot collect all the candies in three passes.</p>
