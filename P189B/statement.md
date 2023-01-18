## Description

<div><p>You have two positive integers <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>h</i></span>. Your task is to count the number of rhombi which have the following properties: </p><ul> <li> Have positive area. </li><li> With vertices at integer points. </li><li> All vertices of the rhombi are located inside or on the border of the rectangle with vertices at points <span class="tex-span">(0, 0)</span>, <span class="tex-span">(<i>w</i>, 0)</span>, <span class="tex-span">(<i>w</i>, <i>h</i>)</span>, <span class="tex-span">(0, <i>h</i>)</span>. In other words, for all vertices <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> of the rhombus the following conditions should fulfill: <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>w</i></span> and <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i></span>. </li><li> Its diagonals are parallel to the axis. </li></ul> <p>Count the number of such rhombi.</p><p>Let us remind you that a <span class="tex-font-style-it">rhombus</span> is a quadrilateral whose four sides all have the same length.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>h</i></span> <span class="tex-span">(1 ≤ <i>w</i>, <i>h</i> ≤ 4000)</span> — the rectangle's sizes.</p></div><div class="output-specification"><p>Print a single number — the number of sought rhombi.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>h</i></span> <span class="tex-span">(1 ≤ <i>w</i>, <i>h</i> ≤ 4000)</span> — the rectangle's sizes.</p>

## Output

<p>Print a single number — the number of sought rhombi.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
2 2

```




```input2
1 2

```




```output1
1

```




```output2
0

```



## Note

<p>In the first example there exists only one such rhombus. Its vertices are located at points <span class="tex-span">(1, 0)</span>, <span class="tex-span">(2, 1)</span>, <span class="tex-span">(1, 2)</span>, <span class="tex-span">(0, 1)</span>.</p>
