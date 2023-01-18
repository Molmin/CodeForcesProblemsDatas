## Description

<div><p>Vasily the bear has a <span class="tex-font-style-it">favorite rectangle</span>, it has one vertex at point <span class="tex-span">(0, 0)</span>, and the opposite vertex at point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. Of course, the sides of Vasya's favorite rectangle are parallel to the coordinate axes. </p><p>Vasya also loves triangles, if the triangles have one vertex at point <span class="tex-span"><i>B</i> = (0, 0)</span>. That's why today he asks you to find two points <span class="tex-span"><i>A</i> = (<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span"><i>C</i> = (<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, such that the following conditions hold:</p><ul> <li> the coordinates of points: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> are integers. Besides, the following inequation holds: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub></span>; </li><li> the triangle formed by point <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>C</i></span> is rectangular and isosceles (<img align="middle" class="tex-formula" src="file://7MUPVwiH.png" style="max-width: 100.0%;max-height: 100.0%;"> is right); </li><li> all points of the favorite rectangle are located inside or on the border of triangle <span class="tex-span"><i>ABC</i></span>; </li><li> the area of triangle <span class="tex-span"><i>ABC</i></span> is as small as possible. </li></ul><p>Help the bear, find the required points. It is not so hard to proof that these points are unique.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>x</i>, <i>y</i></span> <span class="tex-span">( - 10<sup class="upper-index">9</sup> ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup>, <i>x</i> ≠ 0, <i>y</i> ≠ 0)</span>.</p></div><div class="output-specification"><p>Print in the single line four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> — the coordinates of the required points.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>x</i>, <i>y</i></span> <span class="tex-span">( - 10<sup class="upper-index">9</sup> ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup>, <i>x</i> ≠ 0, <i>y</i> ≠ 0)</span>.</p>

## Output

<p>Print in the single line four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> — the coordinates of the required points.</p>





```input1
10 5

```




```input2
-10 5

```




```output1
0 15 15 0

```




```output2
-15 0 0 15

```



## Note

<p><img class="tex-graphics" src="file://gcUWViSa.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><span class="tex-font-size-script">Figure to the first sample</span></p>
