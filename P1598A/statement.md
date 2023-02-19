## Description

<div><p>Monocarp is playing a computer game. Now he wants to complete the first level of this game.</p><p>A level is a rectangular grid of $2$ rows and $n$ columns. Monocarp controls a character, which starts in cell $(1, 1)$&nbsp;— at the intersection of the $1$-st row and the $1$-st column.</p><p>Monocarp's character can move from one cell to another in one step if the cells are adjacent by side and/or corner. Formally, it is possible to move from cell $(x_1, y_1)$ to cell $(x_2, y_2)$ in one step if $|x_1 - x_2| \le 1$ and $|y_1 - y_2| \le 1$. Obviously, it is prohibited to go outside the grid.</p><p>There are traps in some cells. If Monocarp's character finds himself in such a cell, he dies, and the game ends.</p><p>To complete a level, Monocarp's character should reach cell $(2, n)$&nbsp;— at the intersection of row $2$ and column $n$.</p><p>Help Monocarp determine if it is possible to complete the level.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. Then the test cases follow. Each test case consists of three lines.</p><p>The first line contains a single integer $n$ ($3 \le n \le 100$)&nbsp;— the number of columns.</p><p>The next two lines describe the level. The $i$-th of these lines describes the $i$-th line of the level&nbsp;— the line consists of the characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'. The character '<span class="tex-font-style-tt">0</span>' corresponds to a safe cell, the character '<span class="tex-font-style-tt">1</span>' corresponds to a trap cell.</p><p>Additional constraint on the input: cells $(1, 1)$ and $(2, n)$ are safe.</p></div><div class="output-specification"><p>For each test case, output <span class="tex-font-style-tt">YES</span> if it is possible to complete the level, and <span class="tex-font-style-tt">NO</span> otherwise.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. Then the test cases follow. Each test case consists of three lines.</p><p>The first line contains a single integer $n$ ($3 \le n \le 100$)&nbsp;— the number of columns.</p><p>The next two lines describe the level. The $i$-th of these lines describes the $i$-th line of the level&nbsp;— the line consists of the characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'. The character '<span class="tex-font-style-tt">0</span>' corresponds to a safe cell, the character '<span class="tex-font-style-tt">1</span>' corresponds to a trap cell.</p><p>Additional constraint on the input: cells $(1, 1)$ and $(2, n)$ are safe.</p>

## Output

<p>For each test case, output <span class="tex-font-style-tt">YES</span> if it is possible to complete the level, and <span class="tex-font-style-tt">NO</span> otherwise.</p>





```input1
4
3
000
000
4
0011
1100
4
0111
1110
6
010101
101010
```




```output1
YES
YES
NO
YES
```



## Note

<p>Consider the example from the statement.</p><p>In the first test case, one of the possible paths is $(1, 1) \rightarrow (2, 2) \rightarrow (2, 3)$.</p><p>In the second test case, one of the possible paths is $(1, 1) \rightarrow (1, 2) \rightarrow (2, 3) \rightarrow (2, 4)$.</p><p>In the fourth test case, one of the possible paths is $(1, 1) \rightarrow (2, 2) \rightarrow (1, 3) \rightarrow (2, 4) \rightarrow (1, 5) \rightarrow (2, 6)$.</p>
