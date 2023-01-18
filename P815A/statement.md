## Description

<div><p>On the way to school, Karen became fixated on the puzzle game on her phone!</p><center> <img class="tex-graphics" src="file://5LBKrZLU.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The game is played as follows. In each level, you have a grid with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Each cell originally contains the number <span class="tex-span">0</span>.</p><p>One move consists of choosing one row or column, and adding <span class="tex-span">1</span> to all of the cells in that row or column.</p><p>To win the level, after all the moves, the number in the cell at the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column should be equal to <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>.</p><p>Karen is stuck on one level, and wants to know a way to beat this level using the minimum number of moves. Please, help her with this task!</p></div><div class="input-specification"><p>The first line of input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>), the number of rows and the number of columns in the grid, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines each contain <span class="tex-span"><i>m</i></span> integers. In particular, the <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th of these rows contains <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>g</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 500</span>).</p></div><div class="output-specification"><p>If there is an error and it is actually not possible to beat the level, output a single integer <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, on the first line, output a single integer <span class="tex-span"><i>k</i></span>, the minimum number of moves necessary to beat the level.</p><p>The next <span class="tex-span"><i>k</i></span> lines should each contain one of the following, describing the moves in the order they must be done:</p><ul> <li> <span class="tex-font-style-tt">row</span> <span class="tex-span"><i>x</i></span>, (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>) describing a move of the form "choose the <span class="tex-span"><i>x</i></span>-th row". </li><li> <span class="tex-font-style-tt">col</span> <span class="tex-span"><i>x</i></span>, (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>m</i></span>) describing a move of the form "choose the <span class="tex-span"><i>x</i></span>-th column". </li></ul><p>If there are multiple optimal solutions, output any one of them.</p></div>

## Input

<p>The first line of input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>), the number of rows and the number of columns in the grid, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines each contain <span class="tex-span"><i>m</i></span> integers. In particular, the <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th of these rows contains <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>g</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 500</span>).</p>

## Output

<p>If there is an error and it is actually not possible to beat the level, output a single integer <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, on the first line, output a single integer <span class="tex-span"><i>k</i></span>, the minimum number of moves necessary to beat the level.</p><p>The next <span class="tex-span"><i>k</i></span> lines should each contain one of the following, describing the moves in the order they must be done:</p><ul> <li> <span class="tex-font-style-tt">row</span> <span class="tex-span"><i>x</i></span>, (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>) describing a move of the form "choose the <span class="tex-span"><i>x</i></span>-th row". </li><li> <span class="tex-font-style-tt">col</span> <span class="tex-span"><i>x</i></span>, (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>m</i></span>) describing a move of the form "choose the <span class="tex-span"><i>x</i></span>-th column". </li></ul><p>If there are multiple optimal solutions, output any one of them.</p>





```input1
3 5
2 2 2 3 2
0 0 0 1 0
1 1 1 2 1

```




```input2
3 3
0 0 0
0 1 0
0 0 0

```




```input3
3 3
1 1 1
1 1 1
1 1 1

```




```output1
4
row 1
row 1
col 4
row 3

```




```output2
-1

```




```output3
3
row 1
row 2
row 3

```



## Note

<p>In the first test case, Karen has a grid with <span class="tex-span">3</span> rows and <span class="tex-span">5</span> columns. She can perform the following <span class="tex-span">4</span> moves to beat the level:</p><center> <img class="tex-graphics" src="file://fAVKX4ej.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second test case, Karen has a grid with <span class="tex-span">3</span> rows and <span class="tex-span">3</span> columns. It is clear that it is impossible to beat the level; performing any move will create three <span class="tex-span">1</span>s on the grid, but it is required to only have one <span class="tex-span">1</span> in the center.</p><p>In the third test case, Karen has a grid with <span class="tex-span">3</span> rows and <span class="tex-span">3</span> columns. She can perform the following <span class="tex-span">3</span> moves to beat the level:</p><center> <img class="tex-graphics" src="file://VahgZh5o.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that this is not the only solution; another solution, among others, is <span class="tex-font-style-tt">col 1</span>, <span class="tex-font-style-tt">col 2</span>, <span class="tex-font-style-tt">col 3</span>.</p>
