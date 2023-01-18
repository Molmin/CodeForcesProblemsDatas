## Description

<div><p>Shaass thinks a kitchen with all white floor tiles is so boring. His kitchen floor is made of <span class="tex-span"><i>n</i>·<i>m</i></span> square tiles forming a <span class="tex-span"><i>n</i> × <i>m</i></span> rectangle. Therefore he's decided to color some of the tiles in black so that the floor looks like a checkerboard, which is no two side-adjacent tiles should have the same color.</p><p>Shaass wants to use a painter robot to color the tiles. In the beginning the robot is standing in a border tile <span class="tex-span">(<i>x</i><sub class="lower-index"><i>s</i></sub>, <i>y</i><sub class="lower-index"><i>s</i></sub>)</span> facing a diagonal direction (i.e. upper-left, upper-right, down-left or down-right). As the robot walks in the kitchen he paints every tile he passes even if it's painted before. Painting each tile consumes one unit of black paint. If at any moment the robot hits a wall of the kitchen he changes his direction according the reflection rules. Note that a tile gets painted when the robot enters the tile from another tile, in other words changing direction in the same tile doesn't lead to any painting. The first tile the robot is standing on, is also painted.</p><p>The robot stops painting the first moment the floor is checkered. Given the dimensions of the kitchen and the position of the robot, find out the amount of paint the robot consumes before it stops painting the floor.</p><p>Let's consider an examples depicted below.</p><center> <img class="tex-graphics" src="file://88Ktq9C4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>If the robot starts at tile number 1 (the tile <span class="tex-span">(1, 1)</span>) of the left grid heading to down-right it'll pass tiles 1354236 and consumes 7 units of black paint on his way until he stops at tile number 6. But if it starts at tile number 1 in the right grid heading to down-right it will get stuck in a loop painting tiles 1, 2, and 3.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>s</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>s</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>s</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>s</i></sub> ≤ <i>m</i>)</span> and the direction robot is facing initially. Direction is one of the strings: "<span class="tex-font-style-tt">UL</span>" (upper-left direction), "<span class="tex-font-style-tt">UR</span>" (upper-right), "<span class="tex-font-style-tt">DL</span>" (down-left) or "<span class="tex-font-style-tt">DR</span>" (down-right).</p><p>Note, that record <span class="tex-span">(<i>x</i><sub class="lower-index"><i>s</i></sub>, <i>y</i><sub class="lower-index"><i>s</i></sub>)</span> denotes the tile that is located at the <span class="tex-span"><i>x</i><sub class="lower-index"><i>s</i></sub></span>-th row from the top and at the <span class="tex-span"><i>y</i><sub class="lower-index"><i>s</i></sub></span>-th column from the left of the kitchen.</p><p>It's guaranteed that the starting position will be a border tile (a tile with less than four side-adjacent tiles).</p></div><div class="output-specification"><p>Print the amount of paint the robot consumes to obtain a checkered kitchen floor. Or print <span class="tex-font-style-tt">-1</span> if it never happens.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>s</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>s</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>s</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>s</i></sub> ≤ <i>m</i>)</span> and the direction robot is facing initially. Direction is one of the strings: "<span class="tex-font-style-tt">UL</span>" (upper-left direction), "<span class="tex-font-style-tt">UR</span>" (upper-right), "<span class="tex-font-style-tt">DL</span>" (down-left) or "<span class="tex-font-style-tt">DR</span>" (down-right).</p><p>Note, that record <span class="tex-span">(<i>x</i><sub class="lower-index"><i>s</i></sub>, <i>y</i><sub class="lower-index"><i>s</i></sub>)</span> denotes the tile that is located at the <span class="tex-span"><i>x</i><sub class="lower-index"><i>s</i></sub></span>-th row from the top and at the <span class="tex-span"><i>y</i><sub class="lower-index"><i>s</i></sub></span>-th column from the left of the kitchen.</p><p>It's guaranteed that the starting position will be a border tile (a tile with less than four side-adjacent tiles).</p>

## Output

<p>Print the amount of paint the robot consumes to obtain a checkered kitchen floor. Or print <span class="tex-font-style-tt">-1</span> if it never happens.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>





```input1
3 4
1 1 DR

```




```input2
3 4
3 3 DR

```




```input3
3 3
1 1 DR

```




```input4
3 3
1 2 DL

```




```output1
7

```




```output2
11

```




```output3
-1

```




```output4
4

```


