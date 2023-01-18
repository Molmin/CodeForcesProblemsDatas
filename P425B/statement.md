## Description

<div><p>Sereja has an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangular table <span class="tex-span"><i>a</i></span>, each cell of the table contains a zero or a number one. Sereja wants his table to meet the following requirement: each connected component of the same values forms a rectangle with sides parallel to the sides of the table. Rectangles should be filled with cells, that is, if a component form a rectangle of size <span class="tex-span"><i>h</i> × <i>w</i></span>, then the component must contain exactly <span class="tex-span"><i>hw</i></span> cells.</p><p>A connected component of the same values is a set of cells of the table that meet the following conditions:</p><ul> <li> every two cells of the set have the same value; </li><li> the cells of the set form a connected region on the table (two cells are connected if they are adjacent in some row or some column of the table); </li><li> it is impossible to add any cell to the set unless we violate the two previous conditions. </li></ul><p>Can Sereja change the values of at most <span class="tex-span"><i>k</i></span> cells of the table so that the table met the described requirement? What minimum number of table cells should he change in this case?</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100;&nbsp;1 ≤ <i>k</i> ≤ 10)</span>. Next <span class="tex-span"><i>n</i></span> lines describe the table <span class="tex-span"><i>a</i></span>: the <span class="tex-span"><i>i</i></span>-th of them contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>im</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 1)</span> — the values in the cells of the <span class="tex-span"><i>i</i></span>-th row.</p></div><div class="output-specification"><p>Print -1, if it is impossible to meet the requirement. Otherwise, print the minimum number of cells which should be changed.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100;&nbsp;1 ≤ <i>k</i> ≤ 10)</span>. Next <span class="tex-span"><i>n</i></span> lines describe the table <span class="tex-span"><i>a</i></span>: the <span class="tex-span"><i>i</i></span>-th of them contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>im</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 1)</span> — the values in the cells of the <span class="tex-span"><i>i</i></span>-th row.</p>

## Output

<p>Print -1, if it is impossible to meet the requirement. Otherwise, print the minimum number of cells which should be changed.</p>





```input1
5 5 2
1 1 1 1 1
1 1 1 1 1
1 1 0 1 1
1 1 1 1 1
1 1 1 1 1

```




```input2
3 4 1
1 0 0 0
0 1 1 1
1 1 1 0

```




```input3
3 4 1
1 0 0 1
0 1 1 0
1 0 0 1

```




```output1
1

```




```output2
-1

```




```output3
0

```


