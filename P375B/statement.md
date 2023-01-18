## Description

<div><p>You are given a matrix consisting of digits zero and one, its size is <span class="tex-span"><i>n</i> × <i>m</i></span>. You are allowed to rearrange its rows. What is the maximum area of the submatrix that only consists of ones and can be obtained in the given problem by the described operations?</p><p>Let's assume that the rows of matrix <span class="tex-span"><i>a</i></span> are numbered from 1 to <span class="tex-span"><i>n</i></span> from top to bottom and the columns are numbered from 1 to <span class="tex-span"><i>m</i></span> from left to right. A matrix cell on the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column can be represented as <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. Formally, a submatrix of matrix <span class="tex-span"><i>a</i></span> is a group of four integers <span class="tex-span"><i>d</i>, <i>u</i>, <i>l</i>, <i>r</i></span> <span class="tex-span">(1 ≤ <i>d</i> ≤ <i>u</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>m</i>)</span>. We will assume that the submatrix contains cells <span class="tex-span">(<i>i</i>, <i>j</i>)</span> <span class="tex-span">(<i>d</i> ≤ <i>i</i> ≤ <i>u</i>;&nbsp;<i>l</i> ≤ <i>j</i> ≤ <i>r</i>)</span>. The area of the submatrix is the number of cells it contains.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 5000)</span>. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — matrix <span class="tex-span"><i>a</i></span>. Matrix <span class="tex-span"><i>a</i></span> only contains characters: "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". Note that the elements of the matrix follow without any spaces in the lines.</p></div><div class="output-specification"><p>Print a single integer — the area of the maximum obtained submatrix. If we cannot obtain a matrix of numbers one, print 0.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 5000)</span>. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — matrix <span class="tex-span"><i>a</i></span>. Matrix <span class="tex-span"><i>a</i></span> only contains characters: "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". Note that the elements of the matrix follow without any spaces in the lines.</p>

## Output

<p>Print a single integer — the area of the maximum obtained submatrix. If we cannot obtain a matrix of numbers one, print 0.</p>





```input1
1 1
1

```




```input2
2 2
10
11

```




```input3
4 3
100
011
000
101

```




```output1
1

```




```output2
2

```




```output3
2

```


