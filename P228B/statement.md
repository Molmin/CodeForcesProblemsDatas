## Description

<div><p>You've got two rectangular tables with sizes <span class="tex-span"><i>n</i><sub class="lower-index"><i>a</i></sub> × <i>m</i><sub class="lower-index"><i>a</i></sub></span> and <span class="tex-span"><i>n</i><sub class="lower-index"><i>b</i></sub> × <i>m</i><sub class="lower-index"><i>b</i></sub></span> cells. The tables consist of zeroes and ones. We will consider the rows and columns of both tables indexed starting from 1. Then we will define the element of the first table, located at the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column, as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>; we will define the element of the second table, located at the intersection of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column, as <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. </p><p>We will call the pair of integers <span class="tex-span">(<i>x</i>, <i>y</i>)</span> a <span class="tex-font-style-it">shift</span> of the second table relative to the first one. We'll call the <span class="tex-font-style-it">overlap factor</span> of the shift <span class="tex-span">(<i>x</i>, <i>y</i>)</span> value:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://H8zijjQr.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>where the variables <span class="tex-span"><i>i</i>, <i>j</i></span> take only such values, in which the expression <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub>·<i>b</i><sub class="lower-index"><i>i</i> + <i>x</i>, <i>j</i> + <i>y</i></sub></span> makes sense. More formally, inequalities <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i><sub class="lower-index"><i>a</i></sub>, 1 ≤ <i>j</i> ≤ <i>m</i><sub class="lower-index"><i>a</i></sub>, 1 ≤ <i>i</i> + <i>x</i> ≤ <i>n</i><sub class="lower-index"><i>b</i></sub>, 1 ≤ <i>j</i> + <i>y</i> ≤ <i>m</i><sub class="lower-index"><i>b</i></sub></span> must hold. If there are no values of variables <span class="tex-span"><i>i</i>, <i>j</i></span>, that satisfy the given inequalities, the value of the sum is considered equal to 0. </p><p>Your task is to find the shift with the maximum overlap factor among all possible shifts.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>a</i></sub>, <i>m</i><sub class="lower-index"><i>a</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i><sub class="lower-index"><i>a</i></sub>, <i>m</i><sub class="lower-index"><i>a</i></sub> ≤ 50)</span> — the number of rows and columns in the first table. Then <span class="tex-span"><i>n</i><sub class="lower-index"><i>a</i></sub></span> lines contain <span class="tex-span"><i>m</i><sub class="lower-index"><i>a</i></sub></span> characters each — the elements of the first table. Each character is either a "<span class="tex-font-style-tt">0</span>", or a "<span class="tex-font-style-tt">1</span>".</p><p>The next line contains two space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>b</i></sub>, <i>m</i><sub class="lower-index"><i>b</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i><sub class="lower-index"><i>b</i></sub>, <i>m</i><sub class="lower-index"><i>b</i></sub> ≤ 50)</span> — the number of rows and columns in the second table. Then follow the elements of the second table in the format, similar to the first table.</p><p>It is guaranteed that the first table has at least one number "<span class="tex-font-style-tt">1</span>". It is guaranteed that the second table has at least one number "<span class="tex-font-style-tt">1</span>".</p></div><div class="output-specification"><p>Print two space-separated integers <span class="tex-span"><i>x</i>, <i>y</i></span> <span class="tex-span">(|<i>x</i>|, |<i>y</i>| ≤ 10<sup class="upper-index">9</sup>)</span> — a shift with maximum overlap factor. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>a</i></sub>, <i>m</i><sub class="lower-index"><i>a</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i><sub class="lower-index"><i>a</i></sub>, <i>m</i><sub class="lower-index"><i>a</i></sub> ≤ 50)</span> — the number of rows and columns in the first table. Then <span class="tex-span"><i>n</i><sub class="lower-index"><i>a</i></sub></span> lines contain <span class="tex-span"><i>m</i><sub class="lower-index"><i>a</i></sub></span> characters each — the elements of the first table. Each character is either a "<span class="tex-font-style-tt">0</span>", or a "<span class="tex-font-style-tt">1</span>".</p><p>The next line contains two space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>b</i></sub>, <i>m</i><sub class="lower-index"><i>b</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i><sub class="lower-index"><i>b</i></sub>, <i>m</i><sub class="lower-index"><i>b</i></sub> ≤ 50)</span> — the number of rows and columns in the second table. Then follow the elements of the second table in the format, similar to the first table.</p><p>It is guaranteed that the first table has at least one number "<span class="tex-font-style-tt">1</span>". It is guaranteed that the second table has at least one number "<span class="tex-font-style-tt">1</span>".</p>

## Output

<p>Print two space-separated integers <span class="tex-span"><i>x</i>, <i>y</i></span> <span class="tex-span">(|<i>x</i>|, |<i>y</i>| ≤ 10<sup class="upper-index">9</sup>)</span> — a shift with maximum overlap factor. If there are multiple solutions, print any of them.</p>





```input1
3 2
01
10
00
2 3
001
111

```




```input2
3 3
000
010
000
1 1
1

```




```output1
0 1

```




```output2
-1 -1

```


