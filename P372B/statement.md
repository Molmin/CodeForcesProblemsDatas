## Description

<div><p>There is an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangular grid, each cell of the grid contains a single integer: zero or one. Let's call the cell on the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column as <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p><p>Let's define a "rectangle" as four integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ <i>c</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>b</i> ≤ <i>d</i> ≤ <i>m</i>)</span>. Rectangle denotes a set of cells of the grid <span class="tex-span">{(<i>x</i>, <i>y</i>)&nbsp;: &nbsp;<i>a</i> ≤ <i>x</i> ≤ <i>c</i>, <i>b</i> ≤ <i>y</i> ≤ <i>d</i>}</span>. Let's define a "good rectangle" as a rectangle that includes only the cells with zeros.</p><p>You should answer the following <span class="tex-span"><i>q</i></span> queries: calculate the number of good rectangles all of which cells are in the given rectangle.</p></div><div class="input-specification"><p>There are three integers in the first line: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 40, 1 ≤ <i>q</i> ≤ 3·10<sup class="upper-index">5</sup></span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the grid. Consider grid rows are numbered from top to bottom, and grid columns are numbered from left to right. Both columns and rows are numbered starting from 1. </p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains a query — four integers that describe the current rectangle, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ <i>c</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>b</i> ≤ <i>d</i> ≤ <i>m</i>)</span>.</p></div><div class="output-specification"><p>For each query output an answer — a single integer in a separate line.</p></div>

## Input

<p>There are three integers in the first line: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 40, 1 ≤ <i>q</i> ≤ 3·10<sup class="upper-index">5</sup></span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the grid. Consider grid rows are numbered from top to bottom, and grid columns are numbered from left to right. Both columns and rows are numbered starting from 1. </p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains a query — four integers that describe the current rectangle, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ <i>c</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>b</i> ≤ <i>d</i> ≤ <i>m</i>)</span>.</p>

## Output

<p>For each query output an answer — a single integer in a separate line.</p>





```input1
5 5 5
00101
00000
00001
01000
00001
1 2 2 4
4 5 4 5
1 2 5 2
2 2 4 5
4 2 5 3

```




```input2
4 7 5
0000100
0000010
0011000
0000000
1 7 2 7
3 1 3 1
2 3 4 5
1 2 2 7
2 2 4 7

```




```output1
10
1
7
34
5

```




```output2
3
1
16
27
52

```



## Note

<p>For the first example, there is a <span class="tex-span">5 × 5</span> rectangular grid, and the first, the second, and the third queries are represented in the following image.</p><center> <img class="tex-graphics" src="file://swShpcxQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><ul> <li> For the first query, there are <span class="tex-span">10</span> good rectangles, five <span class="tex-span">1 × 1</span>, two <span class="tex-span">2 × 1</span>, two <span class="tex-span">1 × 2</span>, and one <span class="tex-span">1 × 3</span>. </li><li> For the second query, there is only one <span class="tex-span">1 × 1</span> good rectangle. </li><li> For the third query, there are <span class="tex-span">7</span> good rectangles, four <span class="tex-span">1 × 1</span>, two <span class="tex-span">2 × 1</span>, and one <span class="tex-span">3 × 1</span>. </li></ul>
