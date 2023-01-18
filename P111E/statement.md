## Description

<div><p>Little Petya loves playing with rectangles. Mom bought Petya a rectangle divided into cells <span class="tex-span"><i>n</i> × <i>m</i></span> in size (containing <span class="tex-span"><i>n</i></span> rows, <span class="tex-span"><i>m</i></span> columns). Petya marked two different cells of the rectangle and now he is solving the following task:</p><p>Let's define a <span class="tex-font-style-underline">simple path</span> between those two cells as a sequence of distinct cells <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> are the two marked cells. Besides, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> are side-neighboring cells of the path (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span>). Let's denote the path length as number <span class="tex-span"><i>k</i></span> (the sequence length). </p><p>Petya's task is to find the longest simple path's length and to print the path. Help him.</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">4 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the number of rows and the number of columns in the rectangle, correspondingly. The second line contains space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> — the coordinates of the first marked cell. The third line contains space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> — the coordinates of the second marked cell (<span class="tex-span">1 &lt; <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> &lt; <i>n</i>, 1 &lt; <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> &lt; <i>m</i>, <i>x</i><sub class="lower-index">1</sub> ≠ <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">1</sub> ≠ <i>y</i><sub class="lower-index">2</sub></span>).</p><p>The coordinates of a marked cell are a pair of integers <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>, where <span class="tex-span"><i>x</i></span> represents the row's number and <span class="tex-span"><i>y</i></span> represents the column's number. The rows are numbered from top to bottom with consecutive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The columns are numbered from the left to the right by consecutive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p><p>It is guaranteed that the marked cells are not positioned in one row or column.</p></div><div class="output-specification"><p>In the first line print the length of the found path — <span class="tex-span"><i>k</i></span>. In the next lines print <span class="tex-span"><i>k</i></span> pairs of integers, one per line — coordinates of the cells that constitute the found path in the order, in which they follow in the path (the path must go from cell <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> to cell <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>). If there are several solutions, print any of them.</p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">4 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the number of rows and the number of columns in the rectangle, correspondingly. The second line contains space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> — the coordinates of the first marked cell. The third line contains space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> — the coordinates of the second marked cell (<span class="tex-span">1 &lt; <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> &lt; <i>n</i>, 1 &lt; <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> &lt; <i>m</i>, <i>x</i><sub class="lower-index">1</sub> ≠ <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">1</sub> ≠ <i>y</i><sub class="lower-index">2</sub></span>).</p><p>The coordinates of a marked cell are a pair of integers <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>, where <span class="tex-span"><i>x</i></span> represents the row's number and <span class="tex-span"><i>y</i></span> represents the column's number. The rows are numbered from top to bottom with consecutive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The columns are numbered from the left to the right by consecutive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p><p>It is guaranteed that the marked cells are not positioned in one row or column.</p>

## Output

<p>In the first line print the length of the found path — <span class="tex-span"><i>k</i></span>. In the next lines print <span class="tex-span"><i>k</i></span> pairs of integers, one per line — coordinates of the cells that constitute the found path in the order, in which they follow in the path (the path must go from cell <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> to cell <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>). If there are several solutions, print any of them.</p>





```input1
4 4
2 2
3 3

```




```output1
15
2 2
1 2
1 1
2 1
3 1
4 1
4 2
4 3
4 4
3 4
2 4
1 4
1 3
2 3
3 3

```



## Note

<p>The statement test is described in the picture: </p><center> <img class="tex-graphics" src="file://Y3K4yCX1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
