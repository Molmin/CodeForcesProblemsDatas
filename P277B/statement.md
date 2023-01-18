## Description

<div><p>Convexity of a set of points on the plane is the size of the largest subset of points that form a convex polygon. Your task is to build a set of <span class="tex-span"><i>n</i></span> points with the convexity of exactly <span class="tex-span"><i>m</i></span>. Your set of points should not contain three points that lie on a straight line.</p></div><div class="input-specification"><p>The single line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>m</i> ≤ 100, <i>m</i> ≤ <i>n</i> ≤ 2<i>m</i></span>).</p></div><div class="output-specification"><p>If there is no solution, print "<span class="tex-font-style-tt">-1</span>". Otherwise, print <span class="tex-span"><i>n</i></span> pairs of integers — the coordinates of points of any set with the convexity of <span class="tex-span"><i>m</i></span>. The coordinates shouldn't exceed <span class="tex-span">10<sup class="upper-index">8</sup></span> in their absolute value.</p></div>

## Input

<p>The single line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>m</i> ≤ 100, <i>m</i> ≤ <i>n</i> ≤ 2<i>m</i></span>).</p>

## Output

<p>If there is no solution, print "<span class="tex-font-style-tt">-1</span>". Otherwise, print <span class="tex-span"><i>n</i></span> pairs of integers — the coordinates of points of any set with the convexity of <span class="tex-span"><i>m</i></span>. The coordinates shouldn't exceed <span class="tex-span">10<sup class="upper-index">8</sup></span> in their absolute value.</p>





```input1
4 3

```




```input2
6 3

```




```input3
6 6

```




```input4
7 4

```




```output1
0 0
3 0
0 3
1 1

```




```output2
-1

```




```output3
10 0
-10 0
10 1
9 1
9 -1
0 -2

```




```output4
176166 6377
709276 539564
654734 174109
910147 434207
790497 366519
606663 21061
859328 886001

```


