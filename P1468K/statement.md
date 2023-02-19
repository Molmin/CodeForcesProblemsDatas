## Description

<div><p>There is a robot on a checkered field that is endless in all directions. Initially, the robot is located in the cell with coordinates $(0, 0)$. He will execute commands which are described by a string of capital Latin letters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>', '<span class="tex-font-style-tt">U</span>'. When a command is executed, the robot simply moves in the corresponding direction:</p><ul> <li> '<span class="tex-font-style-tt">L</span>': one cell to the left (the $x$-coordinate of the current cell decreases by $1$); </li><li> '<span class="tex-font-style-tt">R</span>': one cell to the right (the $x$-coordinate of the current cell is increased by $1$); </li><li> '<span class="tex-font-style-tt">D</span>': one cell down (the $y$-coordinate of the current cell decreases by $1$); </li><li> '<span class="tex-font-style-tt">U</span>': one cell up (the $y$-coordinate of the current cell is increased by $1$). </li></ul><p>Your task is to put an obstacle in one cell of the field so that after executing the commands, the robot will return to the original cell of its path $(0, 0)$. Of course, an obstacle cannot be placed in the starting cell $(0, 0)$. It is guaranteed that if the obstacle is not placed, then the robot will not return to the starting cell.</p><p>An obstacle affects the movement of the robot in the following way: if it tries to go in a certain direction, and there is an obstacle, then it simply remains in place (the obstacle also remains, that is, it does not disappear).</p><p>Find any such cell of the field (other than $(0, 0)$) that if you put an obstacle there, the robot will return to the cell $(0, 0)$ after the execution of all commands. If there is no solution, then report it.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 500$) — the number of test cases.</p><p>Each test case consists of a single line containing $s$ — the sequence of commands, which are uppercase Latin letters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>', '<span class="tex-font-style-tt">U</span>' only. The length of $s$ is between $1$ and $5000$, inclusive. Additional constraint on $s$: executing this sequence of commands leads the robot to some cell other than $(0, 0)$, if there are no obstacles.</p><p>The sum of lengths of all $s$ in a test doesn't exceed $5000$.</p></div><div class="output-specification"><p>For each test case print a single line:</p><ul> <li> if there is a solution, print two integers $x$ and $y$ ($-10^9 \le x,y \le 10^9$) such that an obstacle in $(x, y)$ will force the robot to return back to the cell $(0, 0)$; </li><li> otherwise, print two zeroes (i. e. <span class="tex-font-style-tt">0 0</span>). </li></ul><p>If there are multiple answers, you can print any of them.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 500$) — the number of test cases.</p><p>Each test case consists of a single line containing $s$ — the sequence of commands, which are uppercase Latin letters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>', '<span class="tex-font-style-tt">U</span>' only. The length of $s$ is between $1$ and $5000$, inclusive. Additional constraint on $s$: executing this sequence of commands leads the robot to some cell other than $(0, 0)$, if there are no obstacles.</p><p>The sum of lengths of all $s$ in a test doesn't exceed $5000$.</p>

## Output

<p>For each test case print a single line:</p><ul> <li> if there is a solution, print two integers $x$ and $y$ ($-10^9 \le x,y \le 10^9$) such that an obstacle in $(x, y)$ will force the robot to return back to the cell $(0, 0)$; </li><li> otherwise, print two zeroes (i. e. <span class="tex-font-style-tt">0 0</span>). </li></ul><p>If there are multiple answers, you can print any of them.</p>





```input1
4
L
RUUDL
LLUU
DDDUUUUU
```




```output1
-1 0
1 2
0 0
0 1
```


