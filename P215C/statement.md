## Description

<div><p>There is a board with a grid consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns, the rows are numbered from <span class="tex-span">1</span> from top to bottom and the columns are numbered from <span class="tex-span">1</span> from left to right. In this grid we will denote the cell that lies on row number <span class="tex-span"><i>i</i></span> and column number <span class="tex-span"><i>j</i></span> as <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p><p>A group of six numbers <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>, <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>)</span>, where <span class="tex-span">0 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i></span>, is a <span class="tex-font-style-it">cross</span>, and there is a set of cells that are assigned to it. Cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> belongs to this set if <span class="tex-font-style-bf">at least one</span> of two conditions are fulfilled:</p><ul> <li> <span class="tex-span">|<i>x</i><sub class="lower-index">0</sub> - <i>x</i>| ≤ <i>a</i></span> and <span class="tex-span">|<i>y</i><sub class="lower-index">0</sub> - <i>y</i>| ≤ <i>b</i></span> </li><li> <span class="tex-span">|<i>x</i><sub class="lower-index">0</sub> - <i>x</i>| ≤ <i>c</i></span> and <span class="tex-span">|<i>y</i><sub class="lower-index">0</sub> - <i>y</i>| ≤ <i>d</i></span> </li></ul><center> <img class="tex-graphics" src="file://3HNZaagi.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> The picture shows the cross <span class="tex-span">(0, 1, 1, 0, 2, 3)</span> on the grid <span class="tex-span">3 × 4</span>. </span> </center><p>Your task is to find the number of different groups of six numbers, <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>, <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>)</span> that determine the crosses of an area equal to <span class="tex-span"><i>s</i></span>, which are placed entirely on the grid. The cross is placed entirely on the grid, if any of its cells is in the range of the grid (that is for each cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> of the cross <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>y</i> ≤ <i>m</i></span> holds). The area of the cross is the number of cells it has.</p><p><span class="tex-font-style-bf">Note that two crosses are considered distinct if the ordered groups of six numbers that denote them are distinct, even if these crosses coincide as sets of points.</span></p></div><div class="input-specification"><p>The input consists of a single line containing three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i>·<i>m</i></span>). The integers are separated by a space.</p></div><div class="output-specification"><p>Print a single integer — the number of distinct groups of six integers that denote crosses with area <span class="tex-span"><i>s</i></span> and that are fully placed on the <span class="tex-span"><i>n</i> × <i>m</i></span> grid.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The input consists of a single line containing three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i>·<i>m</i></span>). The integers are separated by a space.</p>

## Output

<p>Print a single integer — the number of distinct groups of six integers that denote crosses with area <span class="tex-span"><i>s</i></span> and that are fully placed on the <span class="tex-span"><i>n</i> × <i>m</i></span> grid.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
2 2 1

```




```input2
3 4 5

```




```output1
4

```




```output2
4

```



## Note

<p>In the first sample the sought groups of six numbers are: <span class="tex-span">(0, 0, 0, 0, 1, 1)</span>, <span class="tex-span">(0, 0, 0, 0, 1, 2)</span>, <span class="tex-span">(0, 0, 0, 0, 2, 1)</span>, <span class="tex-span">(0, 0, 0, 0, 2, 2)</span>.</p><p>In the second sample the sought groups of six numbers are: <span class="tex-span">(0, 1, 1, 0, 2, 2)</span>, <span class="tex-span">(0, 1, 1, 0, 2, 3)</span>, <span class="tex-span">(1, 0, 0, 1, 2, 2)</span>, <span class="tex-span">(1, 0, 0, 1, 2, 3)</span>.</p>
