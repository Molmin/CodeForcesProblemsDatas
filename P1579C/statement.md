## Description

<div><p>Casimir has a rectangular piece of paper with a checkered field of size $n \times m$. Initially, all cells of the field are white.</p><p>Let us denote the cell with coordinates $i$ vertically and $j$ horizontally by $(i, j)$. The upper left cell will be referred to as $(1, 1)$ and the lower right cell as $(n, m)$.</p><p>Casimir draws <span class="tex-font-style-it">ticks</span> of different sizes on the field. A tick of size $d$ ($d &gt; 0$) with its center in cell $(i, j)$ is drawn as follows: </p><ol> <li> First, the center cell $(i, j)$ is painted black. </li><li> Then exactly $d$ cells on the top-left diagonally to the center and exactly $d$ cells on the top-right diagonally to the center are also painted black. </li><li> That is all the cells with coordinates $(i - h, j \pm h)$ for all $h$ between $0$ and $d$ are painted. In particular, a tick consists of $2d + 1$ black cells. </li></ol><p>An already painted cell will remain black if painted again. Below you can find an example of the $4 \times 9$ box, with two ticks of sizes $2$ and $3$.</p><center> <img class="tex-graphics" src="file://mWSq0gDF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given a description of a checkered field of size $n \times m$. Casimir claims that this field came about after he drew some (possibly $0$) ticks on it. The ticks could be of different sizes, but the size of each tick is at least $k$ (that is, $d \ge k$ for all the ticks).</p><p>Determine whether this field can indeed be obtained by drawing some (possibly none) ticks of sizes $d \ge k$ or not.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number test cases.</p><p>The following lines contain the descriptions of the test cases. </p><p>The first line of the test case description contains the integers $n$, $m$, and $k$ ($1 \le k \le n \le 10$; $1 \le m \le 19$)&nbsp;— the field size and the minimum size of the ticks that Casimir drew. The following $n$ lines describe the field: each line consists of $m$ characters either being '<span class="tex-font-style-tt">.</span>' if the corresponding cell is not yet painted or '<span class="tex-font-style-tt">*</span>' otherwise.</p></div><div class="output-specification"><p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to a test case should be <span class="tex-font-style-tt">YES</span> if the given field can be obtained by drawing ticks of at least the given size and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span>, and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answers).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number test cases.</p><p>The following lines contain the descriptions of the test cases. </p><p>The first line of the test case description contains the integers $n$, $m$, and $k$ ($1 \le k \le n \le 10$; $1 \le m \le 19$)&nbsp;— the field size and the minimum size of the ticks that Casimir drew. The following $n$ lines describe the field: each line consists of $m$ characters either being '<span class="tex-font-style-tt">.</span>' if the corresponding cell is not yet painted or '<span class="tex-font-style-tt">*</span>' otherwise.</p>

## Output

<p>Print $t$ lines, each line containing the answer to the corresponding test case. The answer to a test case should be <span class="tex-font-style-tt">YES</span> if the given field can be obtained by drawing ticks of at least the given size and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span>, and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answers).</p>





```input1
8
2 3 1
*.*
...
4 9 2
*.*.*...*
.*.*...*.
..*.*.*..
.....*...
4 4 1
*.*.
****
.**.
....
5 5 1
.....
*...*
.*.*.
..*.*
...*.
5 5 2
.....
*...*
.*.*.
..*.*
...*.
4 7 1
*.....*
.....*.
..*.*..
...*...
3 3 1
***
***
***
3 5 1
*...*
.***.
.**..
```




```output1
NO
YES
YES
YES
NO
NO
NO
NO
```



## Note

<p>The first sample test case consists of two asterisks neither of which can be independent ticks since ticks of size $0$ don't exist.</p><p>The second sample test case is already described in the statement (check the picture in the statement). This field can be obtained by drawing ticks of sizes $2$ and $3$, as shown in the figure.</p><p>The field in the third sample test case corresponds to three ticks of size $1$. Their center cells are marked with $\color{blue}{\text{blue}}$, $\color{red}{\text{red}}$ and $\color{green}{\text{green}}$ colors: </p><table class="tex-tabular"><tbody><tr><td><span class="tex-font-style-tt">*.*.</span></td></tr><tr><td><span class="tex-font-style-tt">*$\color{blue}{\textbf{*}}$**</span></td></tr><tr><td><span class="tex-font-style-tt">.$\color{green}{\textbf{*}}\color{red}{\textbf{*}}$.</span></td></tr><tr><td><span class="tex-font-style-tt">....</span></td></tr></tbody></table><p></p><p>The field in the fourth sample test case could have been obtained by drawing two ticks of sizes $1$ and $2$. Their vertices are marked below with $\color{blue}{\text{blue}}$ and $\color{red}{\text{red}}$ colors respectively: </p><table class="tex-tabular"><tbody><tr><td><span class="tex-font-style-tt">.....</span></td></tr><tr><td><span class="tex-font-style-tt">*...*</span></td></tr><tr><td><span class="tex-font-style-tt">.*.*.</span></td></tr><tr><td><span class="tex-font-style-tt">..$\color{red}{\textbf{*}}$.*</span></td></tr><tr><td><span class="tex-font-style-tt">...$\color{blue}{\textbf{*}}$.</span></td></tr></tbody></table><p></p><p>The field in the fifth sample test case can not be obtained because $k = 2$, and the last asterisk in the fourth row from the top with coordinates $(4, 5)$ can only be a part of a tick of size $1$.</p><p>The field in the sixth sample test case can not be obtained because the top left asterisk $(1, 1)$ can't be an independent tick, since the sizes of the ticks must be positive, and cannot be part of a tick with the center cell in the last row, since it is separated from it by a gap (a point, '<span class="tex-font-style-tt">.</span>') in $(2, 2)$.</p><p>In the seventh sample test case, similarly, the field can not be obtained by the described process because the asterisks with coordinates $(1, 2)$ (second cell in the first row), $(3, 1)$ and $(3, 3)$ (leftmost and rightmost cells in the bottom) can not be parts of any ticks.</p>
