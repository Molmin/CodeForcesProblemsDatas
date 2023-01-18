## Description

<div><p>Maria participates in a bicycle race.</p><p>The speedway takes place on the shores of Lake Lucerne, just repeating its contour. As you know, the lake shore consists only of straight sections, directed to the north, south, east or west.</p><p>Let's introduce a system of coordinates, directing the <span class="tex-span"><i>Ox</i></span> axis from west to east, and the <span class="tex-span"><i>Oy</i></span> axis from south to north. As a starting position of the race the southernmost point of the track is selected (and if there are several such points, the most western among them). The participants start the race, moving to the north. At all straight sections of the track, the participants travel in one of the four directions (north, south, east or west) and change the direction of movement only in bends between the straight sections. The participants, of course, never turn back, that is, they do not change the direction of movement from north to south or from east to west (or vice versa).</p><p>Maria is still young, so she does not feel confident at some turns. Namely, Maria feels insecure if at a failed or untimely turn, she gets into the water. In other words, Maria considers the turn dangerous if she immediately gets into the water if it is ignored.</p><p>Help Maria get ready for the competition&nbsp;— determine the number of dangerous turns on the track.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of straight sections of the track.</p><p>The following <span class="tex-span">(<i>n</i> + 1)</span>-th line contains pairs of integers <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span"> - 10 000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>). The first of these points is the starting position. The <span class="tex-span"><i>i</i></span>-th straight section of the track begins at the point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> and ends at the point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i> + 1</sub>, <i>y</i><sub class="lower-index"><i>i</i> + 1</sub>)</span>.</p><p>It is guaranteed that:</p><ul> <li> the first straight section is directed to the north; </li><li> the southernmost (and if there are several, then the most western of among them) point of the track is the first point; </li><li> the last point coincides with the first one (i.e., the start position); </li><li> any pair of straight sections of the track has no shared points (except for the neighboring ones, they share exactly one point); </li><li> no pair of points (except for the first and last one) is the same; </li><li> no two adjacent straight sections are directed in the same direction or in opposite directions. </li></ul></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of dangerous turns on the track.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of straight sections of the track.</p><p>The following <span class="tex-span">(<i>n</i> + 1)</span>-th line contains pairs of integers <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span"> - 10 000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>). The first of these points is the starting position. The <span class="tex-span"><i>i</i></span>-th straight section of the track begins at the point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> and ends at the point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i> + 1</sub>, <i>y</i><sub class="lower-index"><i>i</i> + 1</sub>)</span>.</p><p>It is guaranteed that:</p><ul> <li> the first straight section is directed to the north; </li><li> the southernmost (and if there are several, then the most western of among them) point of the track is the first point; </li><li> the last point coincides with the first one (i.e., the start position); </li><li> any pair of straight sections of the track has no shared points (except for the neighboring ones, they share exactly one point); </li><li> no pair of points (except for the first and last one) is the same; </li><li> no two adjacent straight sections are directed in the same direction or in opposite directions. </li></ul>

## Output

<p>Print a single integer&nbsp;— the number of dangerous turns on the track.</p>





```input1
6
0 0
0 1
1 1
1 2
2 2
2 0
0 0

```




```input2
16
1 1
1 5
3 5
3 7
2 7
2 9
6 9
6 7
5 7
5 3
4 3
4 4
3 4
3 2
5 2
5 1
1 1

```




```output1
1

```




```output2
6

```



## Note

<p>The first sample corresponds to the picture:</p><center> <img class="tex-graphics" src="file://ABhMYYh3.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The picture shows that you can get in the water under unfortunate circumstances only at turn at the point <span class="tex-span">(1, 1)</span>. Thus, the answer is <span class="tex-span">1</span>.</p>
