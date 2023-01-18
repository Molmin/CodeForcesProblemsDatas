## Description

<div><p>Victor and Peter are playing hide-and-seek. Peter has hidden, and Victor is to find him. In the room where they are playing, there is only one non-transparent wall and one double-sided mirror. Victor and Peter are points with coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>v</i></sub>, <i>y</i><sub class="lower-index"><i>v</i></sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index"><i>p</i></sub>, <i>y</i><sub class="lower-index"><i>p</i></sub>)</span> respectively. The wall is a segment joining points with coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>w</i>, 1</sub>, <i>y</i><sub class="lower-index"><i>w</i>, 1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index"><i>w</i>, 2</sub>, <i>y</i><sub class="lower-index"><i>w</i>, 2</sub>)</span>, the mirror — a segment joining points <span class="tex-span">(<i>x</i><sub class="lower-index"><i>m</i>, 1</sub>, <i>y</i><sub class="lower-index"><i>m</i>, 1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index"><i>m</i>, 2</sub>, <i>y</i><sub class="lower-index"><i>m</i>, 2</sub>)</span>.</p><p>If an obstacle has a common point with a line of vision, it's considered, that the boys can't see each other with this line of vision. If the mirror has a common point with the line of vision, it's considered, that the boys can see each other in the mirror, i.e. reflection takes place. The reflection process is governed by laws of physics — the angle of incidence is equal to the angle of reflection. The incident ray is in the same half-plane as the reflected ray, relative to the mirror. I.e. to see each other Victor and Peter should be to the same side of the line, containing the mirror (see example 1). If the line of vision is parallel to the mirror, reflection doesn't take place, and the mirror isn't regarded as an obstacle (see example 4).</p><p>Victor got interested if he can see Peter, while standing at the same spot. Help him solve this problem.</p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>v</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>v</i></sub></span> — coordinates of Victor.</p><p>The second line contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>p</i></sub></span> — coordinates of Peter.</p><p>The third line contains 4 numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>w</i>, 1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>w</i>, 1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>w</i>, 2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>w</i>, 2</sub></span> — coordinates of the wall.</p><p>The forth line contains 4 numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>m</i>, 1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>m</i>, 1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>m</i>, 2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>m</i>, 2</sub></span> — coordinates of the mirror.</p><p>All the coordinates are integer numbers, and don't exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> in absolute value. It's guaranteed, that the segments don't have common points, Victor and Peter are not on any of the segments, coordinates of Victor and Peter aren't the same, the segments don't degenerate into points.</p></div><div class="output-specification"><p>Output <span class="tex-font-style-tt">YES</span>, if Victor can see Peter without leaving the initial spot. Otherwise output <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>v</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>v</i></sub></span> — coordinates of Victor.</p><p>The second line contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>p</i></sub></span> — coordinates of Peter.</p><p>The third line contains 4 numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>w</i>, 1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>w</i>, 1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>w</i>, 2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>w</i>, 2</sub></span> — coordinates of the wall.</p><p>The forth line contains 4 numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>m</i>, 1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>m</i>, 1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>m</i>, 2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>m</i>, 2</sub></span> — coordinates of the mirror.</p><p>All the coordinates are integer numbers, and don't exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> in absolute value. It's guaranteed, that the segments don't have common points, Victor and Peter are not on any of the segments, coordinates of Victor and Peter aren't the same, the segments don't degenerate into points.</p>

## Output

<p>Output <span class="tex-font-style-tt">YES</span>, if Victor can see Peter without leaving the initial spot. Otherwise output <span class="tex-font-style-tt">NO</span>.</p>





```input1
-1 3
1 3
0 2 0 4
0 0 0 1

```




```input2
0 0
1 1
0 1 1 0
-100 -100 -101 -101

```




```input3
0 0
1 1
0 1 1 0
-1 1 1 3

```




```input4
0 0
10 0
100 100 101 101
1 0 3 0

```




```output1
NO

```




```output2
NO

```




```output3
YES

```




```output4
YES

```


