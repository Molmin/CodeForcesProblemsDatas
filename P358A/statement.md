## Description

<div><p>Dima and Seryozha live in an ordinary dormitory room for two. One day Dima had a date with his girl and he asked Seryozha to leave the room. As a compensation, Seryozha made Dima do his homework.</p><p>The teacher gave Seryozha the coordinates of <span class="tex-span"><i>n</i></span> distinct points on the abscissa axis and asked to consecutively connect them by semi-circus in a certain order: first connect the first point with the second one, then connect the second point with the third one, then the third one with the fourth one and so on to the <span class="tex-span"><i>n</i></span>-th point. Two points with coordinates <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, 0)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, 0)</span> should be connected by a semi-circle that passes above the abscissa axis with the diameter that coincides with the segment between points. Seryozha needs to find out if the line on the picture intersects itself. For clarifications, see the picture Seryozha showed to Dima (the left picture has self-intersections, the right picture doesn't have any).</p><center> <img class="tex-graphics" src="file://HKDntScR.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Seryozha is not a small boy, so the coordinates of the points can be rather large. Help Dima cope with the problem.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the <span class="tex-span"><i>i</i></span>-th point has coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, 0)</span>. The points are not necessarily sorted by their <span class="tex-span"><i>x</i></span> coordinate.</p></div><div class="output-specification"><p>In the single line print "<span class="tex-font-style-tt">yes</span>" (without the quotes), if the line has self-intersections. Otherwise, print "<span class="tex-font-style-tt">no</span>" (without the quotes).</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the <span class="tex-span"><i>i</i></span>-th point has coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, 0)</span>. The points are not necessarily sorted by their <span class="tex-span"><i>x</i></span> coordinate.</p>

## Output

<p>In the single line print "<span class="tex-font-style-tt">yes</span>" (without the quotes), if the line has self-intersections. Otherwise, print "<span class="tex-font-style-tt">no</span>" (without the quotes).</p>





```input1
4
0 10 5 15

```




```input2
4
0 15 5 10

```




```output1
yes

```




```output2
no

```



## Note

<p>The first test from the statement is on the picture to the left, the second test is on the picture to the right.</p>
