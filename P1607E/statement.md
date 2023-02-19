## Description

<div><p>The robot is located on a checkered rectangular board of size $n \times m$ ($n$ rows, $m$ columns). The rows in the board are numbered from $1$ to $n$ from top to bottom, and the columns&nbsp;— from $1$ to $m$ from left to right.</p><p>The robot is able to move from the current cell to one of the four cells adjacent by side.</p><p>The sequence of commands $s$ executed by the robot is given. Each command is denoted by one of the symbols '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>' or '<span class="tex-font-style-tt">U</span>', and triggers the movement to left, right, down or up, respectively.</p><p>The robot can start its movement in <span class="tex-font-style-bf">any</span> cell. The robot executes the commands starting from the first one, strictly in the order in which they are listed in $s$. If the robot moves beyond the edge of the board, it falls and breaks. A command that causes the robot to break is <span class="tex-font-style-bf">not considered</span> successfully executed.</p><p>The robot's task is to execute as many commands as possible without falling off the board. For example, on board $3 \times 3$, if the robot starts a sequence of actions $s=$"<span class="tex-font-style-tt">RRDLUU</span>" ("right", "right", "down", "left", "up", "up") from the central cell, the robot will perform one command, then the next command will force him to cross the edge. If the robot starts moving from the cell $(2, 1)$ (second row, first column) then all commands will be executed successfully and the robot will stop at the cell $(1, 2)$ (first row, second column).</p><center> <img class="tex-graphics" src="file://dIoY4jDf.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The robot starts from cell $(2, 1)$ (second row, first column). It moves right, right, down, left, up, and up. In this case it ends in the cell $(1, 2)$ (first row, second column).</span> </center><p>Determine the cell from which the robot should start its movement in order to execute as many commands as possible.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases.</p><p>In the description of each test case, the first line contains two integers $n$ and $m$ ($1 \leq n, m \leq 10^6$)&nbsp;— the height and width of the field that the robot is located on. The second line of the description is a string $s$ consisting solely of characters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>' and '<span class="tex-font-style-tt">U</span>'&nbsp;— the sequence of commands the robot executes. The string has a length from $1$ to $10^6$ commands.</p><p>It is guaranteed that the total length of $s$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>Print $t$ lines, each of which contains the answer to the corresponding test case. The answer to the test case are two integers $r$ ($1 \leq r \leq n$) and $c$ ($1 \leq c \leq m$), separated by a space&nbsp;— the coordinates of the cell (row number and column number) from which the robot should start moving to perform as many commands as possible.</p><p>If there are several such cells, you may output any of them.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The next $2t$ lines contain descriptions of the test cases.</p><p>In the description of each test case, the first line contains two integers $n$ and $m$ ($1 \leq n, m \leq 10^6$)&nbsp;— the height and width of the field that the robot is located on. The second line of the description is a string $s$ consisting solely of characters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>' and '<span class="tex-font-style-tt">U</span>'&nbsp;— the sequence of commands the robot executes. The string has a length from $1$ to $10^6$ commands.</p><p>It is guaranteed that the total length of $s$ over all test cases does not exceed $10^6$.</p>

## Output

<p>Print $t$ lines, each of which contains the answer to the corresponding test case. The answer to the test case are two integers $r$ ($1 \leq r \leq n$) and $c$ ($1 \leq c \leq m$), separated by a space&nbsp;— the coordinates of the cell (row number and column number) from which the robot should start moving to perform as many commands as possible.</p><p>If there are several such cells, you may output any of them.</p>





```input1
4
1 1
L
1 2
L
3 3
RRDLUU
4 3
LUURRDDLLLUU
```




```output1
1 1
1 2
2 1
3 2
```


