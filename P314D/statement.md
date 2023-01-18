## Description

<div><p>Sereja placed <span class="tex-span"><i>n</i></span> points on a plane. Now Sereja wants to place on the plane two straight lines, intersecting at a right angle, so that one of the straight lines intersect the <span class="tex-span"><i>Ox</i></span> axis at an angle of <span class="tex-span">45</span> degrees and the maximum distance from the points to the straight lines were minimum. </p><p>In this problem we consider the distance between points <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> equal <span class="tex-span">|<i>x</i><sub class="lower-index">1</sub> - <i>x</i><sub class="lower-index">2</sub>| + |<i>y</i><sub class="lower-index">1</sub> - <i>y</i><sub class="lower-index">2</sub>|</span>. The distance between the point and the straight lines is the minimum distance from the point to some point belonging to one of the lines.</p><p>Help Sereja, find the maximum distance from the points to the optimally located straight lines.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the lines. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>In a single line print a real number — the answer to the problem. Your answer will be considered correct iff its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the lines. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>In a single line print a real number — the answer to the problem. Your answer will be considered correct iff its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
4
0 0
2 0
0 2
2 2

```




```input2
4
1 0
0 1
2 1
1 2

```




```output1
0.000000000000000

```




```output2
1.000000000000000

```


