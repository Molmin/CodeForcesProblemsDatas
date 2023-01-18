## Description

<div><p>Pavel loves grid mazes. A grid maze is an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangle maze where each cell is either empty, or is a wall. You can go from one cell to another only if both cells are empty and have a common side.</p><p>Pavel drew a grid maze with all empty cells forming a connected area. That is, you can go from any empty cell to any other one. Pavel doesn't like it when his maze has too little walls. He wants to turn exactly <span class="tex-span"><i>k</i></span> empty cells into walls so that all the remaining cells still formed a connected area. Help him.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>k</i> &lt; <i>s</i></span>), where <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> are the maze's height and width, correspondingly, <span class="tex-span"><i>k</i></span> is the number of walls Pavel wants to add and letter <span class="tex-span"><i>s</i></span> represents the number of empty cells in the original maze.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters. They describe the original maze. If a character on a line equals "<span class="tex-font-style-tt">.</span>", then the corresponding cell is empty and if the character equals "<span class="tex-font-style-tt">#</span>", then the cell is a wall.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> characters each: the new maze that fits Pavel's requirements. Mark the empty cells that you transformed into walls as "<span class="tex-font-style-tt">X</span>", the other cells must be left without changes (that is, "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">#</span>").</p><p>It is guaranteed that a solution exists. If there are multiple solutions you can output any of them.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>k</i> &lt; <i>s</i></span>), where <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> are the maze's height and width, correspondingly, <span class="tex-span"><i>k</i></span> is the number of walls Pavel wants to add and letter <span class="tex-span"><i>s</i></span> represents the number of empty cells in the original maze.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters. They describe the original maze. If a character on a line equals "<span class="tex-font-style-tt">.</span>", then the corresponding cell is empty and if the character equals "<span class="tex-font-style-tt">#</span>", then the cell is a wall.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> characters each: the new maze that fits Pavel's requirements. Mark the empty cells that you transformed into walls as "<span class="tex-font-style-tt">X</span>", the other cells must be left without changes (that is, "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">#</span>").</p><p>It is guaranteed that a solution exists. If there are multiple solutions you can output any of them.</p>





```input1
3 4 2
#..#
..#.
#...

```




```input2
5 4 5
#...
#.#.
.#..
...#
.#.#

```




```output1
#.X#
X.#.
#...

```




```output2
#XXX
#X#.
X#..
...#
.#.#

```


