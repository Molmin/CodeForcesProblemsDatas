## Description

<div><p><span class="tex-font-style-it">Wherever the destination is, whoever we meet, let's render this song together.</span></p><p>On a Cartesian coordinate plane lies a rectangular stage of size <span class="tex-span"><i>w</i> × <i>h</i></span>, represented by a rectangle with corners <span class="tex-span">(0, 0)</span>, <span class="tex-span">(<i>w</i>, 0)</span>, <span class="tex-span">(<i>w</i>, <i>h</i>)</span> and <span class="tex-span">(0, <i>h</i>)</span>. It can be seen that no collisions will happen before one enters the stage.</p><p>On the sides of the stage stand <span class="tex-span"><i>n</i></span> dancers. The <span class="tex-span"><i>i</i></span>-th of them falls into one of the following groups: </p><ul> <li> <span class="tex-font-style-bf">Vertical</span>: stands at <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, 0)</span>, moves in positive <span class="tex-span"><i>y</i></span> direction (upwards); </li><li> <span class="tex-font-style-bf">Horizontal</span>: stands at <span class="tex-span">(0, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>, moves in positive <span class="tex-span"><i>x</i></span> direction (rightwards). </li></ul><center> <img class="tex-graphics" src="file://BLFZ7uty.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>According to choreography, the <span class="tex-span"><i>i</i></span>-th dancer should stand still for the first <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> milliseconds, and then start moving in the specified direction at <span class="tex-span">1</span> unit per millisecond, until another border is reached. It is guaranteed that no two dancers have the same group, position and waiting time at the same time.</p><p>When two dancers collide (i.e. are on the same point at some time when both of them are moving), they immediately exchange their moving directions and go on.</p><center> <img class="tex-graphics" src="file://noW5Z9Tf.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Dancers stop when a border of the stage is reached. Find out every dancer's stopping position.</p></div><div class="input-specification"><p>The first line of input contains three space-separated positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">2 ≤ <i>w</i>, <i>h</i> ≤ 100 000</span>) — the number of dancers and the width and height of the stage, respectively.</p><p>The following <span class="tex-span"><i>n</i></span> lines each describes a dancer: the <span class="tex-span"><i>i</i></span>-th among them contains three space-separated integers <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 99 999</span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), describing a dancer's group <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub> = 1</span> — vertical, <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub> = 2</span> — horizontal), position, and waiting time. If <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub> = 1</span> then <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = <i>x</i><sub class="lower-index"><i>i</i></sub></span>; otherwise <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>w</i> - 1</span> and <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i> - 1</span>. It is guaranteed that no two dancers have the same group, position and waiting time at the same time.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of which contains two space-separated integers <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> — the stopping position of the <span class="tex-span"><i>i</i></span>-th dancer in the input.</p></div>

## Input

<p>The first line of input contains three space-separated positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">2 ≤ <i>w</i>, <i>h</i> ≤ 100 000</span>) — the number of dancers and the width and height of the stage, respectively.</p><p>The following <span class="tex-span"><i>n</i></span> lines each describes a dancer: the <span class="tex-span"><i>i</i></span>-th among them contains three space-separated integers <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 99 999</span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), describing a dancer's group <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub> = 1</span> — vertical, <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub> = 2</span> — horizontal), position, and waiting time. If <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub> = 1</span> then <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = <i>x</i><sub class="lower-index"><i>i</i></sub></span>; otherwise <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>w</i> - 1</span> and <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i> - 1</span>. It is guaranteed that no two dancers have the same group, position and waiting time at the same time.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of which contains two space-separated integers <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> — the stopping position of the <span class="tex-span"><i>i</i></span>-th dancer in the input.</p>





```input1
8 10 8
1 1 10
1 4 13
1 7 1
1 8 2
2 2 0
2 5 14
2 6 0
2 6 1

```




```input2
3 2 3
1 1 2
2 1 1
1 1 5

```




```output1
4 8
10 5
8 8
10 6
10 2
1 8
7 8
10 6

```




```output2
1 3
2 1
1 3

```



## Note

<p>The first example corresponds to the initial setup in the legend, and the tracks of dancers are marked with different colours in the following figure.</p><center> <img class="tex-graphics" src="file://aB7aLbCC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, no dancers collide.</p>
