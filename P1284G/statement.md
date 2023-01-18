## Description

<div><p>It is only a few days until Seollal (Korean Lunar New Year), and Jaehyun has invited his family to his garden. There are kids among the guests. To make the gathering more fun for the kids, Jaehyun is going to run a game of hide-and-seek.</p><p>The garden can be represented by a $n \times m$ grid of unit cells. Some (possibly zero) cells are blocked by rocks, and the remaining cells are free. Two cells are neighbors if they share an edge. Each cell has up to 4 neighbors: two in the horizontal direction and two in the vertical direction. </p><p>Since the garden is represented as a grid, we can classify the cells in the garden as either "<span class="tex-font-style-tt">black</span>" or "<span class="tex-font-style-tt">white</span>". The top-left cell is black, and two cells which are neighbors must be different colors. Cell indices are 1-based, so the top-left corner of the garden is cell $(1, 1)$.</p><p>Jaehyun wants to turn his garden into a <span class="tex-font-style-it">maze</span> by placing some walls between two cells. Walls can only be placed between neighboring cells. If the wall is placed between two neighboring cells $a$ and $b$, then the two cells $a$ and $b$ are not neighboring from that point. One can walk directly between two neighboring cells if and only if there is no wall directly between them. </p><p>A <span class="tex-font-style-it">maze</span> must have the following property. For each pair of free cells in the maze, there must be exactly one simple path between them. A simple path between cells $a$ and $b$ is a sequence of free cells in which the first cell is $a$, the last cell is $b$, all cells are distinct, and any two consecutive cells are neighbors which are not directly blocked by a wall.</p><p>At first, kids will gather in cell $(1, 1)$, and start the hide-and-seek game. A kid can hide in a cell if and only if that cell is free, it is not $(1, 1)$, and has exactly one free neighbor. Jaehyun planted roses in the black cells, so it's dangerous if the kids hide there. So Jaehyun wants to create a maze where the kids can only hide in white cells.</p><p>You are given the map of the garden as input. Your task is to help Jaehyun create a maze.</p></div><div class="input-specification"><p>Your program will be judged in multiple test cases.</p><p>The first line contains the number of test cases $t$. ($1 \le t \le 100$). Afterward, $t$ test cases with the described format will be given.</p><p>The first line of a test contains two integers $n, m$ ($2 \le n, m \le 20$), the size of the grid.</p><p>In the next $n$ line of a test contains a string of length $m$, consisting of the following characters (without any whitespace): </p><ul> <li> <span class="tex-font-style-tt">O</span>: A free cell. </li><li> <span class="tex-font-style-tt">X</span>: A rock. </li></ul><p>It is guaranteed that the first cell (cell $(1, 1)$) is free, and every free cell is reachable from $(1, 1)$. </p><p><span class="tex-font-style-bf">If $t \geq 2$ is satisfied, then the size of the grid will satisfy $n \le 10, m \le 10$</span>. In other words, if any grid with size $n &gt; 10$ or $m &gt; 10$ is given as an input, then it will be the only input on the test case ($t = 1$).</p></div><div class="output-specification"><p>For each test case, print the following:</p><p>If there are no possible mazes, print a single line <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, print a single line <span class="tex-font-style-tt">YES</span>, followed by a grid of size $(2n-1) \times (2m-1)$ denoting the found maze. The rules for displaying the maze follows. All cells are indexed in 1-base.</p><ul> <li> For all $1 \le i \le n, 1 \le j \le m$, if the cell $(i, j)$ is free cell, print <span class="tex-font-style-tt">'O'</span> in the cell $(2i-1, 2j-1)$. Otherwise, print <span class="tex-font-style-tt">'X'</span> in the cell $(2i-1, 2j-1)$. </li><li> For all $1 \le i \le n, 1 \le j \le m-1$, if the neighboring cell $(i, j), (i, j+1)$ have wall blocking it, print <span class="tex-font-style-tt">' '</span> in the cell $(2i-1, 2j)$. Otherwise, print <span class="tex-font-style-bf">any printable character except spaces</span> in the cell $(2i-1, 2j)$. A printable character has an ASCII code in range $[32, 126]$: This includes spaces and alphanumeric characters. </li><li> For all $1 \le i \le n-1, 1 \le j \le m$, if the neighboring cell $(i, j), (i+1, j)$ have wall blocking it, print <span class="tex-font-style-tt">'&nbsp;'</span> in the cell $(2i, 2j-1)$. Otherwise, print <span class="tex-font-style-bf">any printable character except spaces</span> in the cell $(2i, 2j-1)$ </li><li> For all $1 \le i \le n-1, 1 \le j \le m-1$, print <span class="tex-font-style-bf">any printable character</span> in the cell $(2i, 2j)$. </li></ul><p>Please, be careful about trailing newline characters or spaces. Each row of the grid should contain <span class="tex-font-style-bf">exactly $2m-1$</span> characters, and rows should be separated by a newline character. Trailing spaces must not be omitted in a row.</p></div>

## Input

<p>Your program will be judged in multiple test cases.</p><p>The first line contains the number of test cases $t$. ($1 \le t \le 100$). Afterward, $t$ test cases with the described format will be given.</p><p>The first line of a test contains two integers $n, m$ ($2 \le n, m \le 20$), the size of the grid.</p><p>In the next $n$ line of a test contains a string of length $m$, consisting of the following characters (without any whitespace): </p><ul> <li> <span class="tex-font-style-tt">O</span>: A free cell. </li><li> <span class="tex-font-style-tt">X</span>: A rock. </li></ul><p>It is guaranteed that the first cell (cell $(1, 1)$) is free, and every free cell is reachable from $(1, 1)$. </p><p><span class="tex-font-style-bf">If $t \geq 2$ is satisfied, then the size of the grid will satisfy $n \le 10, m \le 10$</span>. In other words, if any grid with size $n &gt; 10$ or $m &gt; 10$ is given as an input, then it will be the only input on the test case ($t = 1$).</p>

## Output

<p>For each test case, print the following:</p><p>If there are no possible mazes, print a single line <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, print a single line <span class="tex-font-style-tt">YES</span>, followed by a grid of size $(2n-1) \times (2m-1)$ denoting the found maze. The rules for displaying the maze follows. All cells are indexed in 1-base.</p><ul> <li> For all $1 \le i \le n, 1 \le j \le m$, if the cell $(i, j)$ is free cell, print <span class="tex-font-style-tt">'O'</span> in the cell $(2i-1, 2j-1)$. Otherwise, print <span class="tex-font-style-tt">'X'</span> in the cell $(2i-1, 2j-1)$. </li><li> For all $1 \le i \le n, 1 \le j \le m-1$, if the neighboring cell $(i, j), (i, j+1)$ have wall blocking it, print <span class="tex-font-style-tt">' '</span> in the cell $(2i-1, 2j)$. Otherwise, print <span class="tex-font-style-bf">any printable character except spaces</span> in the cell $(2i-1, 2j)$. A printable character has an ASCII code in range $[32, 126]$: This includes spaces and alphanumeric characters. </li><li> For all $1 \le i \le n-1, 1 \le j \le m$, if the neighboring cell $(i, j), (i+1, j)$ have wall blocking it, print <span class="tex-font-style-tt">'&nbsp;'</span> in the cell $(2i, 2j-1)$. Otherwise, print <span class="tex-font-style-bf">any printable character except spaces</span> in the cell $(2i, 2j-1)$ </li><li> For all $1 \le i \le n-1, 1 \le j \le m-1$, print <span class="tex-font-style-bf">any printable character</span> in the cell $(2i, 2j)$. </li></ul><p>Please, be careful about trailing newline characters or spaces. Each row of the grid should contain <span class="tex-font-style-bf">exactly $2m-1$</span> characters, and rows should be separated by a newline character. Trailing spaces must not be omitted in a row.</p>





```input1
4
2 2
OO
OO
3 3
OOO
XOO
OOO
4 4
OOOX
XOOX
OOXO
OOOO
5 6
OOOOOO
OOOOOO
OOOOOO
OOOOOO
OOOOOO
```




```output1
YES
OOO
  O
OOO
NO
YES
OOOOO X
  O O  
X O O X
  O    
OOO X O
O O   O
O OOOOO
YES
OOOOOOOOOOO
  O   O   O
OOO OOO OOO
O   O   O  
OOO OOO OOO
  O   O   O
OOO OOO OOO
O   O   O  
OOO OOO OOO
```


