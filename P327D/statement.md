## Description

<div><p>After too much playing on paper, Iahub has switched to computer games. The game he plays is called "Block Towers". It is played in a rectangular grid with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns (it contains <span class="tex-span"><i>n</i> × <i>m</i></span> cells). The goal of the game is to build your own city. Some cells in the grid are big holes, where Iahub can't build any building. The rest of cells are empty. In some empty cell Iahub can build exactly one tower of two following types:</p><ol> <li> Blue towers. Each has population limit equal to <span class="tex-span">100</span>. </li><li> Red towers. Each has population limit equal to <span class="tex-span">200</span>. However, it can be built in some cell only if in that moment at least one of the neighbouring cells has a Blue Tower. Two cells are neighbours is they share a side. </li></ol><p>Iahub is also allowed to destroy a building from any cell. He can do this operation as much as he wants. After destroying a building, the other buildings are not influenced, and the destroyed cell becomes empty (so Iahub can build a tower in this cell if needed, see the second example for such a case).</p><p>Iahub can convince as many population as he wants to come into his city. So he needs to configure his city to allow maximum population possible. Therefore he should find a sequence of operations that builds the city in an optimal way, so that total population limit is as large as possible.</p><p>He says he's the best at this game, but he doesn't have the optimal solution. Write a program that calculates the optimal one, to show him that he's not as good as he thinks. </p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters, describing the grid. The <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th line is '<span class="tex-font-style-tt">.</span>' if you're allowed to build at the cell with coordinates <span class="tex-span">(<i>i</i>, <i>j</i>)</span> a tower (empty cell) or '<span class="tex-font-style-tt">#</span>' if there is a big hole there. </p></div><div class="output-specification"><p>Print an integer <span class="tex-span"><i>k</i></span> in the first line <span class="tex-span">(0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of operations Iahub should perform to obtain optimal result.</p><p>Each of the following <span class="tex-span"><i>k</i></span> lines must contain a single operation in the following format:</p><ol> <li> «<span class="tex-font-style-tt">B x y</span>» <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i>)</span> — building a blue tower at the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span>; </li><li> «<span class="tex-font-style-tt">R x y</span>» <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i>)</span> — building a red tower at the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span>; </li><li> «<span class="tex-font-style-tt">D x y</span>» <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i>)</span> — destroying a tower at the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. </li></ol><p>If there are multiple solutions you can output any of them. Note, that you shouldn't minimize the number of operations.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters, describing the grid. The <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th line is '<span class="tex-font-style-tt">.</span>' if you're allowed to build at the cell with coordinates <span class="tex-span">(<i>i</i>, <i>j</i>)</span> a tower (empty cell) or '<span class="tex-font-style-tt">#</span>' if there is a big hole there. </p>

## Output

<p>Print an integer <span class="tex-span"><i>k</i></span> in the first line <span class="tex-span">(0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of operations Iahub should perform to obtain optimal result.</p><p>Each of the following <span class="tex-span"><i>k</i></span> lines must contain a single operation in the following format:</p><ol> <li> «<span class="tex-font-style-tt">B x y</span>» <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i>)</span> — building a blue tower at the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span>; </li><li> «<span class="tex-font-style-tt">R x y</span>» <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i>)</span> — building a red tower at the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span>; </li><li> «<span class="tex-font-style-tt">D x y</span>» <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i>)</span> — destroying a tower at the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. </li></ol><p>If there are multiple solutions you can output any of them. Note, that you shouldn't minimize the number of operations.</p>





```input1
2 3
..#
.#.

```




```input2
1 3
...

```




```output1
4
B 1 1
R 1 2
R 2 1
B 2 3

```




```output2
5
B 1 1
B 1 2
R 1 3
D 1 2
R 1 2

```


