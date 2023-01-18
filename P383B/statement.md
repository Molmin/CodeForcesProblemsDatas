## Description

<div><p>Iahub got lost in a very big desert. The desert can be represented as a <span class="tex-span"><i>n</i> × <i>n</i></span> square matrix, where each cell is a zone of the desert. The cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> represents the cell at row <span class="tex-span"><i>i</i></span> and column <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span>. Iahub can go from one cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> only down or right, that is to cells <span class="tex-span">(<i>i</i> + 1, <i>j</i>)</span> or <span class="tex-span">(<i>i</i>, <i>j</i> + 1)</span>. </p><p>Also, there are <span class="tex-span"><i>m</i></span> cells that are occupied by volcanoes, which Iahub cannot enter. </p><p>Iahub is initially at cell <span class="tex-span">(1, 1)</span> and he needs to travel to cell <span class="tex-span">(<i>n</i>, <i>n</i>)</span>. Knowing that Iahub needs <span class="tex-span">1</span> second to travel from one cell to another, find the minimum time in which he can arrive in cell <span class="tex-span">(<i>n</i>, <i>n</i>)</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>)</span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of integers, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>)</span>, representing the coordinates of the volcanoes.</p><p>Consider matrix rows are numbered from 1 to <span class="tex-span"><i>n</i></span> from top to bottom, and matrix columns are numbered from 1 to <span class="tex-span"><i>n</i></span> from left to right. There is no volcano in cell <span class="tex-span">(1, 1)</span>. No two volcanoes occupy the same location. </p></div><div class="output-specification"><p>Print one integer, the minimum time in which Iahub can arrive at cell <span class="tex-span">(<i>n</i>, <i>n</i>)</span>. If no solution exists (there is no path to the final cell), print -1.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>)</span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of integers, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>)</span>, representing the coordinates of the volcanoes.</p><p>Consider matrix rows are numbered from 1 to <span class="tex-span"><i>n</i></span> from top to bottom, and matrix columns are numbered from 1 to <span class="tex-span"><i>n</i></span> from left to right. There is no volcano in cell <span class="tex-span">(1, 1)</span>. No two volcanoes occupy the same location. </p>

## Output

<p>Print one integer, the minimum time in which Iahub can arrive at cell <span class="tex-span">(<i>n</i>, <i>n</i>)</span>. If no solution exists (there is no path to the final cell), print -1.</p>





```input1
4 2
1 3
1 4

```




```input2
7 8
1 6
2 6
3 5
3 6
4 3
5 1
5 2
5 3

```




```input3
2 2
1 2
2 1

```




```output1
6

```




```output2
12

```




```output3
-1

```



## Note

<p>Consider the first sample. A possible road is: <span class="tex-span">(1, 1)</span> <span class="tex-span"> → </span> <span class="tex-span">(1, 2)</span> <span class="tex-span"> → </span> <span class="tex-span">(2, 2)</span> <span class="tex-span"> → </span> <span class="tex-span">(2, 3)</span> <span class="tex-span"> → </span> <span class="tex-span">(3, 3)</span> <span class="tex-span"> → </span> <span class="tex-span">(3, 4)</span> <span class="tex-span"> → </span> <span class="tex-span">(4, 4)</span>.</p>
