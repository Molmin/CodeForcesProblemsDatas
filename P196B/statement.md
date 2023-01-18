## Description

<div><p>We've got a rectangular <span class="tex-span"><i>n</i> × <i>m</i></span>-cell maze. Each cell is either passable, or is a wall (impassable). A little boy found the maze and cyclically tiled a plane with it so that the plane became an infinite maze. Now on this plane cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> is a wall if and only if cell <img align="middle" class="tex-formula" src="file://ExLpYRU1.png" style="max-width: 100.0%;max-height: 100.0%;"> is a wall.</p><p>In this problem <img align="middle" class="tex-formula" src="file://8Js6240K.png" style="max-width: 100.0%;max-height: 100.0%;"> is a remainder of dividing number <span class="tex-span"><i>a</i></span> by number <span class="tex-span"><i>b</i></span>.</p><p>The little boy stood at some cell on the plane and he wondered whether he can walk infinitely far away from his starting position. From cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> he can go to one of the following cells: <span class="tex-span">(<i>x</i>, <i>y</i> - 1)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span>, <span class="tex-span">(<i>x</i> - 1, <i>y</i>)</span> and <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span>, provided that the cell he goes to is not a wall.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1500</span>) — the height and the width of the maze that the boy used to cyclically tile the plane.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the labyrinth. Each character is either a "<span class="tex-font-style-tt">#</span>", that marks a wall, a "<span class="tex-font-style-tt">.</span>", that marks a passable cell, or an "<span class="tex-font-style-tt">S</span>", that marks the little boy's starting point. </p><p>The starting point is a passable cell. It is guaranteed that character "<span class="tex-font-style-tt">S</span>" occurs exactly once in the input.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if the little boy can walk infinitely far from the starting point. Otherwise, print "<span class="tex-font-style-tt">No</span>" (without the quotes).</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1500</span>) — the height and the width of the maze that the boy used to cyclically tile the plane.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the labyrinth. Each character is either a "<span class="tex-font-style-tt">#</span>", that marks a wall, a "<span class="tex-font-style-tt">.</span>", that marks a passable cell, or an "<span class="tex-font-style-tt">S</span>", that marks the little boy's starting point. </p><p>The starting point is a passable cell. It is guaranteed that character "<span class="tex-font-style-tt">S</span>" occurs exactly once in the input.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if the little boy can walk infinitely far from the starting point. Otherwise, print "<span class="tex-font-style-tt">No</span>" (without the quotes).</p>





```input1
5 4
##.#
##S#
#..#
#.##
#..#

```




```input2
5 4
##.#
##S#
#..#
..#.
#.##

```




```output1
Yes

```




```output2
No

```



## Note

<p>In the first sample the little boy can go up for infinitely long as there is a "clear path" that goes vertically. He just needs to repeat the following steps infinitely: up, up, left, up, up, right, up.</p><p>In the second sample the vertical path is blocked. The path to the left doesn't work, too — the next "copy" of the maze traps the boy.</p>
