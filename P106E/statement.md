## Description

<div><p>The Galaxy contains <span class="tex-span"><i>n</i></span> planets, there are many different living creatures inhabiting each planet. And each creature can get into troubles! Space rescuers know it perfectly well and they are always ready to help anyone who really needs help. All you need to do is call for them. </p><p>Now the space rescuers plan to build the largest in the history of the Galaxy rescue station; however, the rescue station's location is yet to be determined. As some cases are real emergencies, the rescuers want to find such a point in the Galaxy from which it would be possible to get to the remotest planet in the minimum possible time. In other words, the rescuers need such point in the space that the distance between it and the planet remotest from it was minimal (if we compare this point with all other possible points in the space). Unfortunately, the rescuers can't sole this problem.</p><p>As the planets are quite remote from each other, they can be considered as points in Euclidean three-dimensional space. The distance between points <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub>, <i>z</i><sub class="lower-index"><i>j</i></sub>)</span> can be calculated by the formula <img align="middle" class="tex-formula" src="file://aFpe6iP5.png" style="max-width: 100.0%;max-height: 100.0%;">. The rescue station can be positioned in any point in the space. It can also coincide with some planet. </p><p>Galaxy is in danger! Save the space rescuers and find the required point for them.</p></div><div class="input-specification"><p>The first line of the input file contains integer <span class="tex-span"><i>n</i></span> — the number of planets (<span class="tex-span">1 ≤ <i>N</i> ≤ 100</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains information about the planets. The <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub></span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th planet (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). No two planets coincide.</p></div><div class="output-specification"><p>Print on the first line of the output file three space-separated real numbers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>z</i><sub class="lower-index">0</sub></span> — the coordinates for the future base. If there are several solutions, you are allowed to print any of them. The answer will be accepted if the distance from this point to the remotest planet will differ from the juries' variant in no more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> in absolute or relative value.</p></div>

## Input

<p>The first line of the input file contains integer <span class="tex-span"><i>n</i></span> — the number of planets (<span class="tex-span">1 ≤ <i>N</i> ≤ 100</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains information about the planets. The <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub></span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th planet (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). No two planets coincide.</p>

## Output

<p>Print on the first line of the output file three space-separated real numbers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>, <i>z</i><sub class="lower-index">0</sub></span> — the coordinates for the future base. If there are several solutions, you are allowed to print any of them. The answer will be accepted if the distance from this point to the remotest planet will differ from the juries' variant in no more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> in absolute or relative value.</p>





```input1
5
5 0 0
-5 0 0
0 3 4
4 -3 0
2 2 -2

```




```output1
0.000 0.000 0.000

```


