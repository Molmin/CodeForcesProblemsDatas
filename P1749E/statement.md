## Description

<div><p>Monocarp is playing Minecraft and wants to build a wall of cacti. He wants to build it on a field of sand of the size of $n \times m$ cells. Initially, there are cacti in some cells of the field. <span class="tex-font-style-bf">Note that, in Minecraft, cacti cannot grow on cells adjacent to each other by side — and the initial field meets this restriction</span>. Monocarp can plant new cacti (they must also fulfil the aforementioned condition). He can't chop down any of the cacti that are already growing on the field — he doesn't have an axe, and the cacti are too prickly for his hands.</p><p>Monocarp believes that the wall is complete if there is no path from the top row of the field to the bottom row, such that: </p><ul> <li> each two consecutive cells in the path are adjacent by side; </li><li> no cell belonging to the path contains a cactus. </li></ul><p>Your task is to plant the minimum number of cacti to build a wall (or to report that this is impossible).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^3$)&nbsp;— number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n, m \le 2 \cdot 10^5$; $n \times m \le 4 \cdot 10^5$)&nbsp;— the number of rows and columns, respectively.</p><p>Then $n$ rows follow, $i$-th row contains a string $s_i$ of length $m$, where $s_{i, j}$ is '<span class="tex-font-style-tt">#</span>', if a cactus grows at the intersection of the $i$-th row and the $j$-th column. Otherwise, $s_{i, j}$ is '<span class="tex-font-style-tt">.</span>'.</p><p>The sum of $n \times m$ over all test cases does not exceed $4 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">NO</span> in the first line if it is impossible to build a cactus wall without breaking the rules. Otherwise, print <span class="tex-font-style-tt">YES</span> in the first line, then print $n$ lines of $m$ characters each&nbsp;— the field itself, where the $j$-th character of the $i$-th line is equal to '<span class="tex-font-style-tt">#</span>', if there is a cactus on the intersection of the $i$-th row and the $j$-th column, otherwise it is '<span class="tex-font-style-tt">.</span>'. If there are multiple optimal answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^3$)&nbsp;— number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n, m \le 2 \cdot 10^5$; $n \times m \le 4 \cdot 10^5$)&nbsp;— the number of rows and columns, respectively.</p><p>Then $n$ rows follow, $i$-th row contains a string $s_i$ of length $m$, where $s_{i, j}$ is '<span class="tex-font-style-tt">#</span>', if a cactus grows at the intersection of the $i$-th row and the $j$-th column. Otherwise, $s_{i, j}$ is '<span class="tex-font-style-tt">.</span>'.</p><p>The sum of $n \times m$ over all test cases does not exceed $4 \cdot 10^5$.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">NO</span> in the first line if it is impossible to build a cactus wall without breaking the rules. Otherwise, print <span class="tex-font-style-tt">YES</span> in the first line, then print $n$ lines of $m$ characters each&nbsp;— the field itself, where the $j$-th character of the $i$-th line is equal to '<span class="tex-font-style-tt">#</span>', if there is a cactus on the intersection of the $i$-th row and the $j$-th column, otherwise it is '<span class="tex-font-style-tt">.</span>'. If there are multiple optimal answers, print any of them.</p>





```input1|2,3,4,9,10,11,12,13,14
4
2 4
.#..
..#.
3 3
#.#
...
.#.
5 5
.....
.....
.....
.....
.....
4 3
#..
.#.
#.#
...
```




```output1
YES
.#.#
#.#.
NO
YES
....#
...#.
..#..
.#...
#....
YES
#..
.#.
#.#
...
```


