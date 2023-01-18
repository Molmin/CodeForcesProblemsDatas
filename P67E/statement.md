## Description

<div><p>In the town of Aalam-Aara (meaning the Light of the Earth), previously there was no crime, no criminals but as the time progressed, sins started creeping into the hearts of once righteous people. Seeking solution to the problem, some of the elders found that as long as the corrupted part of population was kept away from the uncorrupted part, the crimes could be stopped. So, they are trying to set up a compound where they can keep the corrupted people. To ensure that the criminals don't escape the compound, a watchtower needs to be set up, so that they can be watched.</p><p>Since the people of Aalam-Aara aren't very rich, they met up with a merchant from some rich town who agreed to sell them a land-plot which has already a straight line fence <span class="tex-span"><i>AB</i></span> along which a few points are set up where they can put up a watchtower. Your task is to help them find out the number of points on that fence where the tower can be put up, so that all the criminals can be watched from there. Only one watchtower can be set up. A criminal is watchable from the watchtower if the line of visibility from the watchtower to him doesn't cross the plot-edges at any point between him and the tower i.e. as shown in figure 1 below, points <span class="tex-span"><i>X</i></span>, <span class="tex-span"><i>Y</i></span>, <span class="tex-span"><i>C</i></span> and <span class="tex-span"><i>A</i></span> are visible from point <span class="tex-span"><i>B</i></span> but the points <span class="tex-span"><i>E</i></span> and <span class="tex-span"><i>D</i></span> are not.</p><center> <img class="tex-graphics" src="file://zR9Tda5K.png" style="max-width: 100.0%;max-height: 100.0%;">   Figure 1 </center><center> <img class="tex-graphics" src="file://Pl8WkpMU.png" style="max-width: 100.0%;max-height: 100.0%;">   Figure 2 </center><p>Assume that the land plot is in the shape of a polygon and coordinate axes have been setup such that the fence <span class="tex-span"><i>AB</i></span> is parallel to <span class="tex-span"><i>x</i></span>-axis and the points where the watchtower can be set up are the integer points on the line. For example, in given figure 2, watchtower can be setup on any of five integer points on <span class="tex-span"><i>AB</i></span> i.e. <span class="tex-span">(4, 8)</span>, <span class="tex-span">(5, 8)</span>, <span class="tex-span">(6, 8)</span>, <span class="tex-span">(7, 8)</span> or <span class="tex-span">(8, 8)</span>. You can assume that no three consecutive points are collinear and all the corner points other than <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>, lie towards same side of fence <span class="tex-span"><i>AB</i></span>. The given polygon doesn't contain self-intersections.</p></div><div class="input-specification"><p>The first line of the test case will consist of the number of vertices <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1000</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines will contain the coordinates of the vertices in the clockwise order of the polygon. On the <span class="tex-span"><i>i</i></span>-th line are integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) separated by a space.</p><p>The endpoints of the fence <span class="tex-span"><i>AB</i></span> are the first two points, <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p></div><div class="output-specification"><p>Output consists of a single line containing the number of points where the watchtower can be set up.</p></div>

## Input

<p>The first line of the test case will consist of the number of vertices <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1000</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines will contain the coordinates of the vertices in the clockwise order of the polygon. On the <span class="tex-span"><i>i</i></span>-th line are integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) separated by a space.</p><p>The endpoints of the fence <span class="tex-span"><i>AB</i></span> are the first two points, <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p>

## Output

<p>Output consists of a single line containing the number of points where the watchtower can be set up.</p>





```input1
5
4 8
8 8
9 4
4 0
0 4

```




```input2
5
4 8
5 8
5 4
7 4
2 2

```




```output1
5

```




```output2
0

```



## Note

<p>Figure 2 shows the first test case. All the points in the figure are watchable from any point on fence <span class="tex-span"><i>AB</i></span>. Since, <span class="tex-span"><i>AB</i></span> has <span class="tex-span">5</span> integer coordinates, so answer is <span class="tex-span">5</span>.</p><p>For case two, fence <span class="tex-span"><i>CD</i></span> and <span class="tex-span"><i>DE</i></span> are not completely visible, thus answer is <span class="tex-span">0</span>.</p>
