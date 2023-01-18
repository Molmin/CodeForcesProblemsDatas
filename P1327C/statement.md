## Description

<div><p>Petya has a rectangular Board of size $n \times m$. Initially, $k$ chips are placed on the board, $i$-th chip is located in the cell at the intersection of $sx_i$-th row and $sy_i$-th column.</p><p>In one action, Petya can move <span class="tex-font-style-bf">all the chips</span> to the left, right, down or up by $1$ cell.</p><p>If the chip was in the $(x, y)$ cell, then after the operation: </p><ul> <li> left, its coordinates will be $(x, y - 1)$; </li><li> right, its coordinates will be $(x, y + 1)$; </li><li> down, its coordinates will be $(x + 1, y)$; </li><li> up, its coordinates will be $(x - 1, y)$. </li></ul><p>If the chip is located by the wall of the board, and the action chosen by Petya moves it towards the wall, then the chip remains in its current position.</p><p><span class="tex-font-style-bf">Note that several chips can be located in the same cell.</span></p><p>For each chip, Petya chose the position which it should visit. Note that it's not necessary for a chip to end up in this position.</p><p>Since Petya does not have a lot of free time, he is ready to do no more than $2nm$ actions.</p><p>You have to find out what actions Petya should do so that each chip visits the position that Petya selected for it at least once. Or determine that it is not possible to do this in $2nm$ actions.</p></div><div class="input-specification"><p>The first line contains three integers $n, m, k$ ($1 \le n, m, k \le 200$) — the number of rows and columns of the board and the number of chips, respectively.</p><p>The next $k$ lines contains two integers each $sx_i, sy_i$ ($ 1 \le sx_i \le n, 1 \le sy_i \le m$) — the starting position of the $i$-th chip.</p><p>The next $k$ lines contains two integers each $fx_i, fy_i$ ($ 1 \le fx_i \le n, 1 \le fy_i \le m$) — the position that the $i$-chip should visit at least once.</p></div><div class="output-specification"><p>In the first line print the number of operations so that each chip visits the position that Petya selected for it at least once.</p><p>In the second line output the sequence of operations. To indicate operations left, right, down, and up, use the characters $L, R, D, U$ respectively.</p><p>If the required sequence does not exist, print <span class="tex-font-style-tt">-1</span> in the single line.</p></div>

## Input

<p>The first line contains three integers $n, m, k$ ($1 \le n, m, k \le 200$) — the number of rows and columns of the board and the number of chips, respectively.</p><p>The next $k$ lines contains two integers each $sx_i, sy_i$ ($ 1 \le sx_i \le n, 1 \le sy_i \le m$) — the starting position of the $i$-th chip.</p><p>The next $k$ lines contains two integers each $fx_i, fy_i$ ($ 1 \le fx_i \le n, 1 \le fy_i \le m$) — the position that the $i$-chip should visit at least once.</p>

## Output

<p>In the first line print the number of operations so that each chip visits the position that Petya selected for it at least once.</p><p>In the second line output the sequence of operations. To indicate operations left, right, down, and up, use the characters $L, R, D, U$ respectively.</p><p>If the required sequence does not exist, print <span class="tex-font-style-tt">-1</span> in the single line.</p>





```input1
3 3 2
1 2
2 1
3 3
3 2
```




```input2
5 4 3
3 4
3 1
3 3
5 3
1 3
1 4
```




```output1
3
DRD
```




```output2
9
DDLUUUURR
```


