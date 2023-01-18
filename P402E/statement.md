## Description

<div><p>You have matrix <span class="tex-span"><i>a</i></span> of size <span class="tex-span"><i>n</i> × <i>n</i></span>. Let's number the rows of the matrix from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom, let's number the columns from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. Let's use <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> to represent the element on the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column. </p><p>Matrix <span class="tex-span"><i>a</i></span> meets the following two conditions: </p><ul> <li> for any numbers <span class="tex-span"><i>i</i>, <i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>) the following inequality holds: <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> ≥ 0</span>; </li><li> <img align="middle" class="tex-formula" src="file://bcAOrawE.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul><p>Matrix <span class="tex-span"><i>b</i></span> is <span class="tex-font-style-it">strictly positive</span>, if for any numbers <span class="tex-span"><i>i</i>, <i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>) the inequality <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub> &gt; 0</span> holds. You task is to determine if there is such integer <span class="tex-span"><i>k</i> ≥ 1</span>, that matrix <span class="tex-span"><i>a</i><sup class="upper-index"><i>k</i></sup></span> is strictly positive.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>) — the number of rows and columns in matrix <span class="tex-span"><i>a</i></span>.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the description of the rows of matrix <span class="tex-span"><i>a</i></span>. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>in</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 50</span>). It is guaranteed that <img align="middle" class="tex-formula" src="file://qJ3f4R5B.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>If there is a positive integer <span class="tex-span"><i>k</i> ≥ 1</span>, such that matrix <span class="tex-span"><i>a</i><sup class="upper-index"><i>k</i></sup></span> is strictly positive, print "<span class="tex-font-style-tt">YES</span>" (without the quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes). </p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>) — the number of rows and columns in matrix <span class="tex-span"><i>a</i></span>.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the description of the rows of matrix <span class="tex-span"><i>a</i></span>. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>in</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 50</span>). It is guaranteed that <img align="middle" class="tex-formula" src="file://qJ3f4R5B.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>If there is a positive integer <span class="tex-span"><i>k</i> ≥ 1</span>, such that matrix <span class="tex-span"><i>a</i><sup class="upper-index"><i>k</i></sup></span> is strictly positive, print "<span class="tex-font-style-tt">YES</span>" (without the quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes). </p>





```input1
2
1 0
0 1

```




```input2
5
4 5 6 1 2
1 2 3 4 5
6 4 1 2 4
1 1 1 1 1
4 4 4 4 4

```




```output1
NO

```




```output2
YES

```


