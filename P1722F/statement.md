## Description

<div><p>An L-shape is a figure on gridded paper that looks like the first four pictures below. An L-shape contains exactly three shaded cells (denoted by <span class="tex-font-style-tt">*</span>), which can be rotated in any way.</p><center> <img class="tex-graphics" src="file://pLFepDfe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given a rectangular grid. Determine if it contains L-shapes only, where L-shapes can't touch an edge or corner. More formally: </p><ul> <li> Each shaded cell in the grid is part of exactly one L-shape, and </li><li> no two L-shapes are adjacent by edge or corner. </li></ul><p>For example, the last two grids in the picture above <span class="tex-font-style-bf">do not</span> satisfy the condition because the two L-shapes touch by corner and edge, respectively.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 50$)&nbsp;— the number of rows and columns in the grid, respectively.</p><p>Then $n$ lines follow, each containing $m$ characters. Each of these characters is either '<span class="tex-font-style-tt">.</span>' or '<span class="tex-font-style-tt">*</span>'&nbsp;— an empty cell or a shaded cell, respectively.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if the grid is made up of L-shape that don't share edges or corners, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 50$)&nbsp;— the number of rows and columns in the grid, respectively.</p><p>Then $n$ lines follow, each containing $m$ characters. Each of these characters is either '<span class="tex-font-style-tt">.</span>' or '<span class="tex-font-style-tt">*</span>'&nbsp;— an empty cell or a shaded cell, respectively.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if the grid is made up of L-shape that don't share edges or corners, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,4,5,6,7,8,16,17,18,19,25,26,27,28,29,30,35,36,37,42,43,44,45
10
6 10
........**
.**......*
..*..*....
.....**...
...*.....*
..**....**
6 10
....*...**
.**......*
..*..*....
.....**...
...*.....*
..**....**
3 3
...
***
...
4 4
.*..
**..
..**
..*.
5 4
.*..
**..
....
..**
..*.
3 2
.*
**
*.
2 3
*..
.**
3 2
..
**
*.
3 3
.**
*.*
**.
3 3
..*
.**
..*
```




```output1
YES
NO
NO
NO
YES
NO
NO
YES
NO
NO
```


