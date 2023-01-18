## Description

<div><p>You play a computer game. Your character stands on some level of a multilevel ice cave. In order to move on forward, you need to descend one level lower and the only way to do this is to fall through the ice.</p><p>The level of the cave where you are is a rectangular square grid of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Each cell consists either from intact or from cracked ice. From each cell you can move to cells that are side-adjacent with yours (due to some limitations of the game engine you cannot make jumps on the same place, i.e. jump from a cell to itself). If you move to the cell with cracked ice, then your character falls down through it and if you move to the cell with intact ice, then the ice on this cell becomes cracked.</p><p>Let's number the rows with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom and the columns with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> from left to right. Let's denote a cell on the intersection of the <span class="tex-span"><i>r</i></span>-th row and the <span class="tex-span"><i>c</i></span>-th column as <span class="tex-span">(<i>r</i>, <i>c</i>)</span>. </p><p>You are staying in the cell <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> and this cell is cracked because you've just fallen here from a higher level. You need to fall down through the cell <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span> since the exit to the next level is there. Can you do this?</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>)&nbsp;— the number of rows and columns in the cave description.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines describes the initial state of the level of the cave, each line consists of <span class="tex-span"><i>m</i></span> characters "<span class="tex-font-style-tt">.</span>" (that is, intact ice) and "<span class="tex-font-style-tt">X</span>" (cracked ice).</p><p>The next line contains two integers, <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ <i>m</i></span>)&nbsp;— your initial coordinates. It is guaranteed that the description of the cave contains character '<span class="tex-font-style-tt">X</span>' in cell <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span>, that is, the ice on the starting cell is initially cracked.</p><p>The next line contains two integers <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>)&nbsp;— the coordinates of the cell through which you need to fall. The final cell may coincide with the starting one.</p></div><div class="output-specification"><p>If you can reach the destination, print '<span class="tex-font-style-tt">YES</span>', otherwise print '<span class="tex-font-style-tt">NO</span>'.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>)&nbsp;— the number of rows and columns in the cave description.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines describes the initial state of the level of the cave, each line consists of <span class="tex-span"><i>m</i></span> characters "<span class="tex-font-style-tt">.</span>" (that is, intact ice) and "<span class="tex-font-style-tt">X</span>" (cracked ice).</p><p>The next line contains two integers, <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ <i>m</i></span>)&nbsp;— your initial coordinates. It is guaranteed that the description of the cave contains character '<span class="tex-font-style-tt">X</span>' in cell <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span>, that is, the ice on the starting cell is initially cracked.</p><p>The next line contains two integers <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>)&nbsp;— the coordinates of the cell through which you need to fall. The final cell may coincide with the starting one.</p>

## Output

<p>If you can reach the destination, print '<span class="tex-font-style-tt">YES</span>', otherwise print '<span class="tex-font-style-tt">NO</span>'.</p>





```input1
4 6
X...XX
...XX.
.X..X.
......
1 6
2 2

```




```input2
5 4
.X..
...X
X.X.
....
.XX.
5 3
1 1

```




```input3
4 7
..X.XX.
.XX..X.
X...X..
X......
2 2
1 6

```




```output1
YES

```




```output2
NO

```




```output3
YES

```



## Note

<p>In the first sample test one possible path is:</p><p><img align="middle" class="tex-formula" src="file://LvGbyO5F.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>After the first visit of cell <span class="tex-span">(2, 2)</span> the ice on it cracks and when you step there for the second time, your character falls through the ice as intended.</p>
