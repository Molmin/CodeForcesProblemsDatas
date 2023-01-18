## Description

<div><p>Vivek has encountered a problem. He has a maze that can be represented as an $n \times m$ grid. Each of the grid cells may represent the following:</p><ul> <li> Empty&nbsp;— '<span class="tex-font-style-tt">.</span>' </li><li> Wall&nbsp;— '<span class="tex-font-style-tt">#</span>' </li><li> Good person &nbsp;— '<span class="tex-font-style-tt">G</span>' </li><li> Bad person&nbsp;— '<span class="tex-font-style-tt">B</span>' </li></ul><p>The only escape from the maze is at cell $(n, m)$.</p><p>A person can move to a cell only if it shares a side with their current cell and does not contain a wall. Vivek wants to block some of the empty cells by replacing them with walls in such a way, that all the good people are able to escape, while none of the bad people are able to. A cell that initially contains '<span class="tex-font-style-tt">G</span>' or '<span class="tex-font-style-tt">B</span>' <span class="tex-font-style-bf">cannot be blocked</span> and <span class="tex-font-style-bf">can be travelled through</span>.</p><p>Help him determine if there exists a way to replace some (zero or more) empty cells with walls to satisfy the above conditions.</p><p><span class="tex-font-style-bf">It is guaranteed that the cell $(n,m)$ is empty.</span> Vivek can also block this cell.</p></div><div class="input-specification"><p>The first line contains one integer $t$ $(1 \le t \le 100)$&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $m$ $(1 \le n, m \le 50)$&nbsp;— the number of rows and columns in the maze.</p><p>Each of the next $n$ lines contain $m$ characters. They describe the layout of the maze. If a character on a line equals '<span class="tex-font-style-tt">.</span>', the corresponding cell is empty. If it equals '<span class="tex-font-style-tt">#</span>', the cell has a wall. '<span class="tex-font-style-tt">G</span>' corresponds to a good person and '<span class="tex-font-style-tt">B</span>' corresponds to a bad person.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">Yes</span>" if there exists a way to replace some empty cells with walls to satisfy the given conditions. Otherwise print "<span class="tex-font-style-tt">No</span>"</p><p>You may print every letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains one integer $t$ $(1 \le t \le 100)$&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $m$ $(1 \le n, m \le 50)$&nbsp;— the number of rows and columns in the maze.</p><p>Each of the next $n$ lines contain $m$ characters. They describe the layout of the maze. If a character on a line equals '<span class="tex-font-style-tt">.</span>', the corresponding cell is empty. If it equals '<span class="tex-font-style-tt">#</span>', the cell has a wall. '<span class="tex-font-style-tt">G</span>' corresponds to a good person and '<span class="tex-font-style-tt">B</span>' corresponds to a bad person.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">Yes</span>" if there exists a way to replace some empty cells with walls to satisfy the given conditions. Otherwise print "<span class="tex-font-style-tt">No</span>"</p><p>You may print every letter in any case (upper or lower).</p>





```input1
6
1 1
.
1 2
G.
2 2
#B
G.
2 3
G.#
B#.
3 3
#B.
#..
GG.
2 2
#B
B.
```




```output1
Yes
Yes
No
No
Yes
Yes
```



## Note

<p>For the first and second test cases, all conditions are already satisfied.</p><p>For the third test case, there is only one empty cell $(2,2)$, and if it is replaced with a wall then the good person at $(1,2)$ will not be able to escape.</p><p>For the fourth test case, the good person at $(1,1)$ cannot escape.</p><p>For the fifth test case, Vivek can block the cells $(2,3)$ and $(2,2)$.</p><p>For the last test case, Vivek can block the destination cell $(2, 2)$.</p>
