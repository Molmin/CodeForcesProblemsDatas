## Description

<div><p>There is a grid with $n$ rows and $m$ columns, and three types of cells: </p><ul> <li> An empty cell, denoted with '<span class="tex-font-style-tt">.</span>'. </li><li> A stone, denoted with '<span class="tex-font-style-tt">*</span>'. </li><li> An obstacle, denoted with the lowercase Latin letter '<span class="tex-font-style-tt">o</span>'. </li></ul><p>All stones fall down until they meet the floor (the bottom row), an obstacle, or other stone which is already immovable. (In other words, all the stones just fall down as long as they can fall.)</p><p>Simulate the process. What does the resulting grid look like?</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 50$)&nbsp;— the number of rows and the number of columns in the grid, respectively.</p><p>Then $n$ lines follow, each containing $m$ characters. Each of these characters is either '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">*</span>', or '<span class="tex-font-style-tt">o</span>'&nbsp;— an empty cell, a stone, or an obstacle, respectively.</p></div><div class="output-specification"><p>For each test case, output a grid with $n$ rows and $m$ columns, showing the result of the process.</p><p><span class="tex-font-style-bf">You don't need to output a new line after each test, it is in the samples just for clarity.</span></p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 50$)&nbsp;— the number of rows and the number of columns in the grid, respectively.</p><p>Then $n$ lines follow, each containing $m$ characters. Each of these characters is either '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">*</span>', or '<span class="tex-font-style-tt">o</span>'&nbsp;— an empty cell, a stone, or an obstacle, respectively.</p>

## Output

<p>For each test case, output a grid with $n$ rows and $m$ columns, showing the result of the process.</p><p><span class="tex-font-style-bf">You don't need to output a new line after each test, it is in the samples just for clarity.</span></p>





```input1
3
6 10
.*.*....*.
.*.......*
...o....o.
.*.*....*.
..........
.o......o*
2 9
...***ooo
.*o.*o.*o
5 5
*****
*....
*****
....*
*****
```




```output1
..........
...*....*.
.*.o....o.
.*........
.*......**
.o.*....o*

....**ooo
.*o**o.*o

.....
*...*
*****
*****
*****
```


