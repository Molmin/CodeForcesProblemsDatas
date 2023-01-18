## Description

<div><p>You are given matrix <span class="tex-span"><i>a</i></span> of size <span class="tex-span"><i>n</i> × <i>m</i></span>, its elements are integers. We will assume that the rows of the matrix are numbered from top to bottom from 1 to <span class="tex-span"><i>n</i></span>, the columns are numbered from left to right from 1 to <span class="tex-span"><i>m</i></span>. We will denote the element on the intersecting of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column as <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span>.</p><p>We'll call submatrix <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>j</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, <i>j</i><sub class="lower-index">2</sub></span> <span class="tex-span">(1 ≤ <i>i</i><sub class="lower-index">1</sub> ≤ <i>i</i><sub class="lower-index">2</sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>j</i><sub class="lower-index">1</sub> ≤ <i>j</i><sub class="lower-index">2</sub> ≤ <i>m</i>)</span> such elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> of the given matrix that <span class="tex-span"><i>i</i><sub class="lower-index">1</sub> ≤ <i>i</i> ≤ <i>i</i><sub class="lower-index">2</sub></span> AND <span class="tex-span"><i>j</i><sub class="lower-index">1</sub> ≤ <i>j</i> ≤ <i>j</i><sub class="lower-index">2</sub></span>. We'll call the area of the submatrix number <span class="tex-span">(<i>i</i><sub class="lower-index">2</sub> - <i>i</i><sub class="lower-index">1</sub> + 1)·(<i>j</i><sub class="lower-index">2</sub> - <i>j</i><sub class="lower-index">1</sub> + 1)</span>. We'll call a submatrix inhomogeneous, if all its elements are distinct.</p><p>Find the largest (in area) inhomogenous submatrix of the given matrix.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 400</span>)&nbsp;— the number of rows and columns of the matrix, correspondingly.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 160000</span>)&nbsp;— the elements of the matrix.</p></div><div class="output-specification"><p>Print a single integer — the area of the optimal inhomogenous submatrix.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 400</span>)&nbsp;— the number of rows and columns of the matrix, correspondingly.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 160000</span>)&nbsp;— the elements of the matrix.</p>

## Output

<p>Print a single integer — the area of the optimal inhomogenous submatrix.</p>





```input1
3 3
1 3 1
4 5 6
2 6 1

```




```input2
3 4
5 2 3 1
3 3 5 3
4 4 4 5

```




```input3
2 6
1 2 3 4 5 6
8 6 7 8 9 1

```




```output1
6

```




```output2
4

```




```output3
8

```


