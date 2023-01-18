## Description

<div><p>Everyone knows that computers become faster and faster. Recently Berland scientists have built a machine that can move itself back in time!</p><p>More specifically, it works as follows. It has an infinite grid and a robot which stands on one of the cells. Each cell of the grid can either be empty or contain <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>. The machine also has a program which consists of instructions, which are being handled one by one. Each instruction is represented by exactly one symbol (letter or digit) and takes exactly one unit of time (say, second) to be performed, except the last type of operation (it's described below). Here they are:</p><ul> <li> <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>: the robot places this number into the cell he is currently at. If this cell wasn't empty before the operation, its previous number is replaced anyway. </li><li> <span class="tex-font-style-tt">e</span>: the robot <span class="tex-font-style-bf">e</span>rases the number into the cell he is at. </li><li> <span class="tex-font-style-tt">l</span>, <span class="tex-font-style-tt">r</span>, <span class="tex-font-style-tt">u</span> or <span class="tex-font-style-tt">d</span>: the robot goes one cell to the <span class="tex-font-style-bf">l</span>eft/<span class="tex-font-style-bf">r</span>ight/<span class="tex-font-style-bf">u</span>p/<span class="tex-font-style-bf">d</span>own. </li><li> <span class="tex-font-style-tt">s</span>: the robot <span class="tex-font-style-bf">s</span>tays where he is for a unit of time. </li><li> <span class="tex-font-style-tt">t</span>: let $x$ be $0$, if the cell with the robot is empty, otherwise let $x$ be one more than the digit in this cell (that is, $x = 1$ if the digit in this cell is $0$, and $x = 2$ if the digit is $1$). Then the machine <span class="tex-font-style-bf">t</span>ravels $x$ seconds back in time. Note that this doesn't change the instructions order, but it changes the position of the robot and the numbers in the grid as they were $x$ units of time ago. You can consider this instruction to be equivalent to a <span class="tex-font-style-tt">Ctrl-Z</span> pressed $x$ times. </li></ul><p>For example, let the board be completely empty, and the program be <span class="tex-font-style-tt">sr1t0</span>. Let the robot initially be at $(0, 0)$.</p><ul> <li> [now is the moment $0$, the command is <span class="tex-font-style-tt">s</span>]: we do nothing. </li><li> [now is the moment $1$, the command is <span class="tex-font-style-tt">r</span>]: we are now at $(1, 0)$. </li><li> [now is the moment $2$, the command is <span class="tex-font-style-tt">1</span>]: we are at $(1, 0)$, and this cell contains $1$. </li><li> [now is the moment $3$, the command is <span class="tex-font-style-tt">t</span>]: we travel $1 + 1 = 2$ moments back, that is, to the moment $1$. </li><li> [now is the moment $1$, the command is <span class="tex-font-style-tt">0</span>]: we are again at $(0, 0)$, and the board is clear again, but after we follow this instruction, this cell has $0$ in it. We've just rewritten the history. The consequences of the third instruction have never happened. </li></ul><p>Now Berland scientists want to use their machine in practice. For example, they want to be able to add two integers.</p><p>Assume that the initial state of the machine is as follows:</p><ul> <li> One positive integer is written in binary on the grid in such a way that its right bit is at the cell $(0, 1)$, from left to right from the highest bit to the lowest bit. </li><li> The other positive integer is written in binary on the grid in such a way that its right bit is at the cell $(0, 0)$, from left to right from the highest bit to the lowest bit. </li><li> All the other cells are empty. </li><li> The robot is at $(0, 0)$. </li><li> We consider this state to be always in the past; that is, if you manage to travel to any negative moment, the board was always as described above, and the robot was at $(0, 0)$ for eternity. </li></ul><p>You are asked to write a program after which</p><ul> <li> The robot stands on a non-empty cell, </li><li> If we read the number starting from the cell with the robot and moving to the right until the first empty cell, this will be $a + b$ in binary, from the highest bit to the lowest bit. </li></ul><p>Note that there are no restrictions on other cells. In particular, there may be a digit just to the left to the robot after all instructions.</p><p>In each test you are given up to $1000$ pairs $(a, b)$, and your program must work for all these pairs. Also since the machine's memory is not very big, your program must consist of no more than $10^5$ instructions.</p></div><div class="input-specification"><p>The first line contains the only integer $t$ ($1\le t\le 1000$) standing for the number of testcases. Each of the next $t$ lines consists of two positive integers $a$ and $b$ ($1\le a, b &lt; 2^{30}$) in decimal.</p></div><div class="output-specification"><p>Output the only line consisting of no more than $10^5$ symbols from <span class="tex-font-style-tt">01eslrudt</span> standing for your program.</p><p>Note that formally you may output different programs for different tests.</p></div>

## Input

<p>The first line contains the only integer $t$ ($1\le t\le 1000$) standing for the number of testcases. Each of the next $t$ lines consists of two positive integers $a$ and $b$ ($1\le a, b &lt; 2^{30}$) in decimal.</p>

## Output

<p>Output the only line consisting of no more than $10^5$ symbols from <span class="tex-font-style-tt">01eslrudt</span> standing for your program.</p><p>Note that formally you may output different programs for different tests.</p>





```input1
2
123456789 987654321
555555555 555555555

```




```output1
0l1l1l0l0l0l1l1l1l0l1l0l1l1l0l0l0l1l0l1l1l1l0l0l0l1l0l0l0l0l1l0lr

```


