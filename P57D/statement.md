## Description

<div><p>Stewie the Rabbit explores a new parallel universe. This two dimensional universe has the shape of a rectangular grid, containing <span class="tex-span"><i>n</i></span> lines and <span class="tex-span"><i>m</i></span> columns. The universe is very small: one cell of the grid can only contain one particle. Each particle in this universe is either static or dynamic. Each static particle always remains in one and the same position. Due to unintelligible gravitation laws no two static particles in the parallel universe can be present in one column or row, and they also can't be present in the diagonally <span class="tex-font-style-bf">adjacent</span> cells. A dynamic particle appears in a random empty cell, randomly chooses the destination cell (destination cell may coincide with the start cell, see the samples) and moves there along the shortest path through the cells, unoccupied by the static particles. All empty cells have the same probability of being selected as the beginning or end of the path. Having reached the destination cell, the particle disappears. Only one dynamic particle can exist at one moment of time. This particle can move from a cell to a cell if they have an adjacent side, and this transition takes exactly one galactic second. Stewie got interested in what is the average lifespan of one particle in the given universe.</p></div><div class="input-specification"><p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) which represent the sizes of the universe. The next <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> symbols each describe the universe without dynamic particles — the <span class="tex-span"><i>j</i></span>-th symbol of the <span class="tex-span"><i>i</i></span>-th line equals to <span class="tex-font-style-tt">'X'</span> if the cell is occupied by a static particle, and to <span class="tex-font-style-tt">'.'</span> if it is empty. It is guaranteed that the described universe satisfies the properties described above, that is no two static particles can be in one column or in one row, besides, they can't be positioned in the diagonally adjacent cells.</p></div><div class="output-specification"><p>You have to print on a single line a single number which is the average life span of a particle with an accuracy of at least 6 decimal places.</p><p>The answer will be accepted if it is within <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> of absolute or relative error from the correct answer.</p></div>

## Input

<p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) which represent the sizes of the universe. The next <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> symbols each describe the universe without dynamic particles — the <span class="tex-span"><i>j</i></span>-th symbol of the <span class="tex-span"><i>i</i></span>-th line equals to <span class="tex-font-style-tt">'X'</span> if the cell is occupied by a static particle, and to <span class="tex-font-style-tt">'.'</span> if it is empty. It is guaranteed that the described universe satisfies the properties described above, that is no two static particles can be in one column or in one row, besides, they can't be positioned in the diagonally adjacent cells.</p>

## Output

<p>You have to print on a single line a single number which is the average life span of a particle with an accuracy of at least 6 decimal places.</p><p>The answer will be accepted if it is within <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> of absolute or relative error from the correct answer.</p>





```input1
2 2
..
.X

```




```input2
3 3
...
.X.
...

```




```output1
0.888888888889

```




```output2
2.000000000000

```


