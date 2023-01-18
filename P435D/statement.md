## Description

<div><p>You are given an <span class="tex-span"><i>n</i> × <i>m</i></span> grid, some of its nodes are black, the others are white. Moreover, it's not an ordinary grid — each unit square of the grid has painted diagonals.</p><p>The figure below is an example of such grid of size <span class="tex-span">3 × 5</span>. Four nodes of this grid are black, the other <span class="tex-span">11</span> nodes are white.</p><center> <img class="tex-graphics" src="file://eDxAyEkm.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Your task is to count the number of such triangles on the given grid that:</p><ul> <li> the corners match the white nodes, and the area is positive; </li><li> all sides go along the grid lines (horizontal, vertical or diagonal); </li><li> no side contains black nodes. </li></ul></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 400)</span>. Each of the following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters (zeros and ones) — the description of the grid. If the <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th line equals zero, then the node on the <span class="tex-span"><i>i</i></span>-th horizontal line and on the <span class="tex-span"><i>j</i></span>-th vertical line is painted white. Otherwise, the node is painted black.</p><p>The horizontal lines are numbered starting from one from top to bottom, the vertical lines are numbered starting from one from left to right. </p></div><div class="output-specification"><p>Print a single integer — the number of required triangles.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 400)</span>. Each of the following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters (zeros and ones) — the description of the grid. If the <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th line equals zero, then the node on the <span class="tex-span"><i>i</i></span>-th horizontal line and on the <span class="tex-span"><i>j</i></span>-th vertical line is painted white. Otherwise, the node is painted black.</p><p>The horizontal lines are numbered starting from one from top to bottom, the vertical lines are numbered starting from one from left to right. </p>

## Output

<p>Print a single integer — the number of required triangles.</p>





```input1
3 5
10000
10010
00001

```




```input2
2 2
00
00

```




```input3
2 2
11
11

```




```output1
20

```




```output2
4

```




```output3
0

```



## Note

<p>The figure below shows red and blue triangles. They are the examples of the required triangles in the first sample. One of the invalid triangles is painted green. It is invalid because not all sides go along the grid lines.</p><center> <img class="tex-graphics" src="file://GbBrCUOm.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
