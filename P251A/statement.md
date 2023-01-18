## Description

<div><p>Little Petya likes points a lot. Recently his mom has presented him <span class="tex-span"><i>n</i></span> points lying on the line <span class="tex-span"><i>OX</i></span>. Now Petya is wondering in how many ways he can choose three distinct points so that the distance between the two farthest of them doesn't exceed <span class="tex-span"><i>d</i></span>.</p><p>Note that the order of the points inside the group of three chosen points doesn't matter.</p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>, their absolute value doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> — the <span class="tex-span"><i>x</i></span>-coordinates of the points that Petya has got.</p><p>It is guaranteed that the coordinates of the points in the input <span class="tex-font-style-bf">strictly increase</span>.</p></div><div class="output-specification"><p>Print a single integer — the number of groups of three points, where the distance between two farthest points doesn't exceed <span class="tex-span"><i>d</i></span>.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>, their absolute value doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> — the <span class="tex-span"><i>x</i></span>-coordinates of the points that Petya has got.</p><p>It is guaranteed that the coordinates of the points in the input <span class="tex-font-style-bf">strictly increase</span>.</p>

## Output

<p>Print a single integer — the number of groups of three points, where the distance between two farthest points doesn't exceed <span class="tex-span"><i>d</i></span>.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
4 3
1 2 3 4

```




```input2
4 2
-3 -2 -1 0

```




```input3
5 19
1 10 20 30 50

```




```output1
4

```




```output2
2

```




```output3
1

```



## Note

<p>In the first sample any group of three points meets our conditions.</p><p>In the seconds sample only 2 groups of three points meet our conditions: <span class="tex-font-style-tt">{-3, -2, -1}</span> and <span class="tex-font-style-tt">{-2, -1, 0}</span>.</p><p>In the third sample only one group does: <span class="tex-font-style-tt">{1, 10, 20}</span>.</p>
