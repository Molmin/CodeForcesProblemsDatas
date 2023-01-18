## Description

<div><p>Polycarp takes part in a quadcopter competition. According to the rules a flying robot should:</p><ul> <li> start the race from some point of a field, </li><li> go around the flag, </li><li> close cycle returning back to the starting point. </li></ul><p>Polycarp knows the coordinates of the starting point (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub></span>) and the coordinates of the point where the flag is situated (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>). Polycarp’s quadcopter can fly only parallel to the sides of the field each tick changing exactly one coordinate by <span class="tex-span">1</span>. It means that in one tick the quadcopter can fly from the point (<span class="tex-span"><i>x</i>, <i>y</i></span>) to any of four points: (<span class="tex-span"><i>x</i> - 1, <i>y</i></span>), (<span class="tex-span"><i>x</i> + 1, <i>y</i></span>), (<span class="tex-span"><i>x</i>, <i>y</i> - 1</span>) or (<span class="tex-span"><i>x</i>, <i>y</i> + 1</span>).</p><p>Thus the quadcopter path is a closed cycle starting and finishing in (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub></span>) and containing the point (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>) strictly inside.</p><center> <img class="tex-graphics" src="file://xFHpHOaF.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The picture corresponds to the first example: the starting (and finishing) point is in (<span class="tex-span">1, 5</span>) and the flag is in (<span class="tex-span">5, 2</span>).</span> </center><p>What is the minimal length of the quadcopter path?</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> (<span class="tex-span"> - 100 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub> ≤ 100</span>) — coordinates of the quadcopter starting (and finishing) point.</p><p>The second line contains two integer numbers <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 100 ≤ <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 100</span>) — coordinates of the flag.</p><p>It is guaranteed that the quadcopter starting point and the flag do not coincide.</p></div><div class="output-specification"><p>Print the length of minimal path of the quadcopter to surround the flag and return back.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> (<span class="tex-span"> - 100 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub> ≤ 100</span>) — coordinates of the quadcopter starting (and finishing) point.</p><p>The second line contains two integer numbers <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 100 ≤ <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 100</span>) — coordinates of the flag.</p><p>It is guaranteed that the quadcopter starting point and the flag do not coincide.</p>

## Output

<p>Print the length of minimal path of the quadcopter to surround the flag and return back.</p>





```input1
1 5
5 2

```




```input2
0 1
0 0

```




```output1
18

```




```output2
8

```


