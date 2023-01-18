## Description

<div><p>You are given a square matrix consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns. We assume that the rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom and the columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. Some cells (<span class="tex-span"><i>n</i> - 1</span> cells in total) of the the matrix are filled with ones, the remaining cells are filled with zeros. We can apply the following operations to the matrix:</p><ol> <li> Swap <span class="tex-span"><i>i</i></span>-th and <span class="tex-span"><i>j</i></span>-th rows of the matrix; </li><li> Swap <span class="tex-span"><i>i</i></span>-th and <span class="tex-span"><i>j</i></span>-th columns of the matrix. </li></ol><p>You are asked to transform the matrix into a special form using these operations. In that special form all the ones must be in the cells that lie below the main diagonal. Cell of the matrix, which is located on the intersection of the <span class="tex-span"><i>i</i></span>-th row and of the <span class="tex-span"><i>j</i></span>-th column, lies below the main diagonal if <span class="tex-span"><i>i</i> &gt; <i>j</i></span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 1000)</span> — the number of rows and columns. Then follow <span class="tex-span"><i>n</i> - 1</span> lines that contain one's positions, one per line. Each position is described by two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i>)</span>, separated by a space. A pair <span class="tex-span">(<i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub>)</span> means that the cell, which is located on the intersection of the <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span>-th row and of the <span class="tex-span"><i>y</i><sub class="lower-index"><i>k</i></sub></span>-th column, contains one.</p><p>It is guaranteed that all positions are distinct.</p></div><div class="output-specification"><p>Print the description of your actions. These actions should transform the matrix to the described special form.</p><p>In the first line you should print a non-negative integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(<i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of actions. In each of the next <span class="tex-span"><i>m</i></span> lines print three space-separated integers <span class="tex-span"><i>t</i>, <i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 2, 1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>, <i>i</i> ≠ <i>j</i>)</span>, where <span class="tex-span"><i>t</i> = 1</span> if you want to swap rows, <span class="tex-span"><i>t</i> = 2</span> if you want to swap columns, and <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> denote the numbers of rows or columns respectively.</p><p>Please note, that you do not need to minimize the number of operations, but their number should not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. If there are several solutions, you may print any of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 1000)</span> — the number of rows and columns. Then follow <span class="tex-span"><i>n</i> - 1</span> lines that contain one's positions, one per line. Each position is described by two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i>)</span>, separated by a space. A pair <span class="tex-span">(<i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub>)</span> means that the cell, which is located on the intersection of the <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span>-th row and of the <span class="tex-span"><i>y</i><sub class="lower-index"><i>k</i></sub></span>-th column, contains one.</p><p>It is guaranteed that all positions are distinct.</p>

## Output

<p>Print the description of your actions. These actions should transform the matrix to the described special form.</p><p>In the first line you should print a non-negative integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(<i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of actions. In each of the next <span class="tex-span"><i>m</i></span> lines print three space-separated integers <span class="tex-span"><i>t</i>, <i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 2, 1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>, <i>i</i> ≠ <i>j</i>)</span>, where <span class="tex-span"><i>t</i> = 1</span> if you want to swap rows, <span class="tex-span"><i>t</i> = 2</span> if you want to swap columns, and <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> denote the numbers of rows or columns respectively.</p><p>Please note, that you do not need to minimize the number of operations, but their number should not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. If there are several solutions, you may print any of them.</p>





```input1
2
1 2

```




```input2
3
3 1
1 3

```




```input3
3
2 1
3 2

```




```output1
2
2 1 2
1 1 2

```




```output2
3
2 2 3
1 1 3
1 1 2

```




```output3
0

```


