## Description

<div><p>One day a bear lived on the <span class="tex-span"><i>Oxy</i></span> axis. He was afraid of the dark, so he couldn't move at night along the plane points that aren't lit. One day the bear wanted to have a night walk from his house at point <span class="tex-span">(<i>l</i>, 0)</span> to his friend's house at point <span class="tex-span">(<i>r</i>, 0)</span>, along the segment of length <span class="tex-span">(<i>r</i> - <i>l</i>)</span>. Of course, if he wants to make this walk, he needs each point of the segment to be lit. That's why the bear called his friend (and yes, in the middle of the night) asking for a very delicate favor.</p><p>The <span class="tex-span"><i>Oxy</i></span> axis contains <span class="tex-span"><i>n</i></span> floodlights. Floodlight <span class="tex-span"><i>i</i></span> is at point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> and can light any angle of the plane as large as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> degree with vertex at point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. The bear asked his friend to turn the floodlights so that he (the bear) could go as far away from his house as possible during the walking along the segment. His kind friend agreed to fulfill his request. And while he is at it, the bear wonders: what is the furthest he can go away from his house? Hep him and find this distance.</p><p>Consider that the plane has no obstacles and no other light sources besides the floodlights. The bear's friend cannot turn the floodlights during the bear's walk. Assume that after all the floodlights are turned in the correct direction, the bear goes for a walk and his friend goes to bed.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 20;&nbsp; - 10<sup class="upper-index">5</sup> ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contain three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1000;&nbsp;1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000;&nbsp;1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 90)</span> — the floodlights' description. </p><p>Note that two floodlights can be at the same point of the plane.</p></div><div class="output-specification"><p>Print a single real number — the answer to the problem. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 20;&nbsp; - 10<sup class="upper-index">5</sup> ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contain three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1000;&nbsp;1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000;&nbsp;1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 90)</span> — the floodlights' description. </p><p>Note that two floodlights can be at the same point of the plane.</p>

## Output

<p>Print a single real number — the answer to the problem. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2 3 5
3 1 45
5 1 45

```




```input2
1 0 1
1 1 30

```




```input3
1 0 1
1 1 45

```




```input4
1 0 2
0 2 90

```




```output1
2.000000000

```




```output2
0.732050808

```




```output3
1.000000000

```




```output4
2.000000000

```



## Note

<p>In the first sample, one of the possible solutions is: </p><center> <img class="tex-graphics" src="file://c2BXTVwp.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample, a single solution is: </p><center> <img class="tex-graphics" src="file://zZuvf58b.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third sample, a single solution is: </p><center> <img class="tex-graphics" src="file://q38HEzwq.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
