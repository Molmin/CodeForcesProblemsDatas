## Description

<div><p>The robot is located on a checkered rectangular board of size $n \times m$ ($n$ rows, $m$ columns). The rows in the board are numbered from $1$ to $n$ from top to bottom, and the columns&nbsp;— from $1$ to $m$ from left to right.</p><p>The robot is able to move from the current cell to one of the four cells adjacent by side.</p><p>Each cell has one of the symbols '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>' or '<span class="tex-font-style-tt">U</span>' written on it, indicating the direction in which the robot will move when it gets in that cell&nbsp;— left, right, down or up, respectively.</p><p>The robot can start its movement in any cell. He then moves to the adjacent square in the direction indicated on the current square in one move. </p><ul> <li> If the robot moves beyond the edge of the board, it falls and breaks. </li><li> If the robot appears in the cell it already visited before, it breaks (it stops and doesn't move anymore). </li></ul><p>Robot can choose any cell as the starting cell. Its goal is to make the maximum number of steps before it breaks or stops.</p><p>Determine from which square the robot should start its movement in order to execute as many commands as possible. A command is considered successfully completed if the robot has moved from the square on which that command was written (it does not matter whether to another square or beyond the edge of the board).</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10000$)&nbsp;— the number of test cases in the test.</p><p>Each test case's description is preceded by a blank line. Next is a line that contains integers $n$ and $m$ ($1 \le n \le 2000$; $1 \le m \le 2000$)&nbsp;— the height and width of the board. This line followed by $n$ lines, the $i$-th of which describes the $i$-th line of the board. Each of them is exactly $m$ letters long and consists of symbols '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>' and '<span class="tex-font-style-tt">U</span>'.</p><p>It is guaranteed that the sum of sizes of all boards in the input does not exceed $4\cdot10^6$.</p></div><div class="output-specification"><p>For each test case, output three integers $r$, $c$ and $d$ ($1 \le r \le n$; $1 \le c \le m$; $d \ge 0$), which denote that the robot should start moving from cell $(r, c)$ to make the maximum number of moves $d$. If there are several answers, output any of them.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10000$)&nbsp;— the number of test cases in the test.</p><p>Each test case's description is preceded by a blank line. Next is a line that contains integers $n$ and $m$ ($1 \le n \le 2000$; $1 \le m \le 2000$)&nbsp;— the height and width of the board. This line followed by $n$ lines, the $i$-th of which describes the $i$-th line of the board. Each of them is exactly $m$ letters long and consists of symbols '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>' and '<span class="tex-font-style-tt">U</span>'.</p><p>It is guaranteed that the sum of sizes of all boards in the input does not exceed $4\cdot10^6$.</p>

## Output

<p>For each test case, output three integers $r$, $c$ and $d$ ($1 \le r \le n$; $1 \le c \le m$; $d \ge 0$), which denote that the robot should start moving from cell $(r, c)$ to make the maximum number of moves $d$. If there are several answers, output any of them.</p>





```input1
7

1 1
R

1 3
RRL

2 2
DL
RU

2 2
UD
RU

3 2
DL
UL
RU

4 4
RRRD
RUUD
URUD
ULLR

4 4
DDLU
RDDU
UUUU
RDLD
```




```output1
1 1 1
1 1 3
1 1 4
2 1 3
3 1 5
4 3 12
1 1 4
```


