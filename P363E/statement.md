## Description

<div><p>Let's assume that we are given an <span class="tex-span"><i>n</i> × <i>m</i></span> table filled by integers. We'll mark a cell in the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column as <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. Thus, <span class="tex-span">(1, 1)</span> is the upper left cell of the table and <span class="tex-span">(<i>n</i>, <i>m</i>)</span> is the lower right cell. We'll assume that a circle of radius <span class="tex-span"><i>r</i></span> with the center in cell <span class="tex-span">(<i>i</i><sub class="lower-index">0</sub>, <i>j</i><sub class="lower-index">0</sub>)</span> is a set of such cells <span class="tex-span">(<i>i</i>, <i>j</i>)</span> that <img align="middle" class="tex-formula" src="file://tiGqILSo.png" style="max-width: 100.0%;max-height: 100.0%;">. We'll consider only the circles that do not go beyond the limits of the table, that is, for which <span class="tex-span"><i>r</i> + 1 ≤ <i>i</i><sub class="lower-index">0</sub> ≤ <i>n</i> - <i>r</i></span> and <span class="tex-span"><i>r</i> + 1 ≤ <i>j</i><sub class="lower-index">0</sub> ≤ <i>m</i> - <i>r</i></span>. </p><center> <img class="tex-graphics" src="file://PdsnmAkN.png" style="max-width: 100.0%;max-height: 100.0%;">  A circle of radius 3 with the center at <span class="tex-span">(4, 5)</span>. </center><p>Find two such non-intersecting circles of the given radius <span class="tex-span"><i>r</i></span> that the sum of numbers in the cells that belong to these circles is maximum. Two circles intersect if there is a cell that belongs to both circles. As there can be more than one way to choose a pair of circles with the maximum sum, we will also be interested in the number of such pairs. Calculate the number of unordered pairs of circles, for instance, a pair of circles of radius 2 with centers at <span class="tex-span">(3, 4)</span> and <span class="tex-span">(7, 7)</span> is the same pair as the pair of circles of radius 2 with centers at <span class="tex-span">(7, 7)</span> and <span class="tex-span">(3, 4)</span>. </p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 500</span>, <span class="tex-span"><i>r</i> ≥ 0</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers from 1 to 1000 each — the elements of the table. The rows of the table are listed from top to bottom at the elements in the rows are listed from left to right. It is guaranteed that there is at least one circle of radius <span class="tex-span"><i>r</i></span>, not going beyond the table limits. </p></div><div class="output-specification"><p>Print two integers — the maximum sum of numbers in the cells that are located into two non-intersecting circles and the number of pairs of non-intersecting circles with the maximum sum. If there isn't a single pair of non-intersecting circles, print <span class="tex-font-style-tt">0 0</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 500</span>, <span class="tex-span"><i>r</i> ≥ 0</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers from 1 to 1000 each — the elements of the table. The rows of the table are listed from top to bottom at the elements in the rows are listed from left to right. It is guaranteed that there is at least one circle of radius <span class="tex-span"><i>r</i></span>, not going beyond the table limits. </p>

## Output

<p>Print two integers — the maximum sum of numbers in the cells that are located into two non-intersecting circles and the number of pairs of non-intersecting circles with the maximum sum. If there isn't a single pair of non-intersecting circles, print <span class="tex-font-style-tt">0 0</span>.</p>





```input1
2 2 0
1 2
2 4

```




```input2
5 6 1
4 2 1 3 2 6
2 3 2 4 7 2
5 2 2 1 1 3
1 4 3 3 6 4
5 1 4 2 3 2

```




```input3
3 3 1
1 2 3
4 5 6
7 8 9

```




```output1
6 2

```




```output2
34 3

```




```output3
0 0

```


