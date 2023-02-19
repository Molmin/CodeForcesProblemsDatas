## Description

<div><p>Sir Monocarp Hamilton is planning to paint his wall. The wall can be represented as a grid, consisting of $2$ rows and $m$ columns. Initially, the wall is completely white.</p><p>Monocarp wants to paint a black picture on the wall. In particular, he wants cell $(i, j)$ (the $j$-th cell in the $i$-th row) to be colored black, if $c_{i, j} =$ '<span class="tex-font-style-tt">B</span>', and to be left white, if $c_{i, j} =$ '<span class="tex-font-style-tt">W</span>'. Additionally, he wants each column to have at least one black cell, so, for each $j$, the following constraint is satisfied: $c_{1, j}$, $c_{2, j}$ or both of them will be equal to '<span class="tex-font-style-tt">B</span>'.</p><p>In order for the picture to turn out smooth, Monocarp wants to place down a paint brush in some cell $(x_1, y_1)$ and move it along the path $(x_1, y_1), (x_2, y_2), \dots, (x_k, y_k)$ so that: </p><ul> <li> for each $i$, $(x_i, y_i)$ and $(x_{i+1}, y_{i+1})$ share a common side; </li><li> all black cells appear in the path <span class="tex-font-style-bf">exactly once</span>; </li><li> white cells don't appear in the path. </li></ul><p>Determine if Monocarp can paint the wall.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of columns in the wall.</p><p>The $i$-th of the next two lines contains a string $c_i$, consisting of $m$ characters, where each character is either '<span class="tex-font-style-tt">B</span>' or '<span class="tex-font-style-tt">W</span>'. $c_{i, j}$ is '<span class="tex-font-style-tt">B</span>', if the cell $(i, j)$ should be colored black, and '<span class="tex-font-style-tt">W</span>', if the cell $(i, j)$ should be left white.</p><p><span class="tex-font-style-bf">Additionally, for each $j$, the following constraint is satisfied: $c_{1, j}$, $c_{2, j}$ or both of them are equal to '<span class="tex-font-style-tt">B</span>'.</span></p><p>The sum of $m$ over all testcases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if Monocarp can paint a wall. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of columns in the wall.</p><p>The $i$-th of the next two lines contains a string $c_i$, consisting of $m$ characters, where each character is either '<span class="tex-font-style-tt">B</span>' or '<span class="tex-font-style-tt">W</span>'. $c_{i, j}$ is '<span class="tex-font-style-tt">B</span>', if the cell $(i, j)$ should be colored black, and '<span class="tex-font-style-tt">W</span>', if the cell $(i, j)$ should be left white.</p><p><span class="tex-font-style-bf">Additionally, for each $j$, the following constraint is satisfied: $c_{1, j}$, $c_{2, j}$ or both of them are equal to '<span class="tex-font-style-tt">B</span>'.</span></p><p>The sum of $m$ over all testcases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if Monocarp can paint a wall. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1|2,3,4,8,9,10,14,15,16
6
3
WBB
BBW
1
B
B
5
BWBWB
BBBBB
2
BW
WB
5
BBBBW
BWBBB
6
BWBBWB
BBBBBB
```




```output1
YES
YES
NO
NO
NO
YES
```



## Note

<p>In the first testcase, Monocarp can follow a path $(2, 1)$, $(2, 2)$, $(1, 2)$, $(1, 3)$ with his brush. All black cells appear in the path exactly once, no white cells appear in the path.</p><p>In the second testcase, Monocarp can follow a path $(1, 1)$, $(2, 1)$.</p><p>In the third testcase: </p><ul> <li> the path $(1, 1)$, $(2, 1)$, $(2, 2)$, $(2, 3)$, $(1, 3)$, $(2, 4)$, $(2, 5)$, $(1, 5)$ doesn't suffice because a pair of cells $(1, 3)$ and $(2, 4)$ doesn't share a common side; </li><li> the path $(1, 1)$, $(2, 1)$, $(2, 2)$, $(2, 3)$, $(1, 3)$, $(2, 3)$, $(2, 4)$, $(2, 5)$, $(1, 5)$ doesn't suffice because cell $(2, 3)$ is visited twice; </li><li> the path $(1, 1)$, $(2, 1)$, $(2, 2)$, $(2, 3)$, $(2, 4)$, $(2, 5)$, $(1, 5)$ doesn't suffice because a black cell $(1, 3)$ doesn't appear in the path; </li><li> the path $(1, 1)$, $(2, 1)$, $(2, 2)$, $(2, 3)$, $(2, 4)$, $(2, 5)$, $(1, 5)$, $(1, 4)$, $(1, 3)$ doesn't suffice because a white cell $(1, 4)$ appears in the path. </li></ul>
