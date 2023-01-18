## Description

<div><p>So, the Berland is at war with its eternal enemy Flatland again, and Vasya, an accountant, was assigned to fulfil his duty to the nation. </p><p>Right now the situation in Berland is dismal — their both cities are surrounded! The armies of flatlanders stand on the borders of circles, the circles' centers are in the surrounded cities. At any moment all points of the flatland ring can begin to move quickly in the direction of the city — that's the strategy the flatlanders usually follow when they besiege cities.</p><p>The berlanders are sure that they can repel the enemy's attack if they learn the exact time the attack starts. For that they need to construct a radar that would register any movement at the distance of at most <span class="tex-span"><i>r</i></span> from it. Thus, we can install a radar at such point, that at least one point of the enemy ring will be in its detecting range (that is, at a distance of at most <span class="tex-span"><i>r</i></span>). Then the radar can immediately inform about the enemy's attack. </p><p>Due to the newest technologies, we can place a radar at any point without any problems. But the problem is that the berlanders have the time to make only one radar. Besides, the larger the detection radius <span class="tex-span">(<i>r</i>)</span> is, the more the radar costs.</p><p>That's why Vasya's task (that is, your task) is to find the minimum possible detection radius for the radar. In other words, your task is to find the minimum radius <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>r</i> ≥ 0)</span> such, that a radar with radius <span class="tex-span"><i>r</i></span> can be installed at some point and it can register <span class="tex-font-style-bf">the start of the movements</span> of both flatland rings from that point. </p><p>In this problem you can consider the cities as material points, the attacking enemy rings - as circles with centers in the cities, the radar's detection range — as a disk (including the border) with the center at the point where the radar is placed.</p></div><div class="input-specification"><p>The input files consist of two lines. Each line represents the city and the flatland ring that surrounds it as three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">4</sup>;&nbsp;1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> — the city's coordinates and the distance from the city to the flatlanders, correspondingly.</p><p>It is guaranteed that the cities are located at different points.</p></div><div class="output-specification"><p>Print a single real number — the minimum detection radius of the described radar. The answer is considered correct if the absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The input files consist of two lines. Each line represents the city and the flatland ring that surrounds it as three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">4</sup>;&nbsp;1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> — the city's coordinates and the distance from the city to the flatlanders, correspondingly.</p><p>It is guaranteed that the cities are located at different points.</p>

## Output

<p>Print a single real number — the minimum detection radius of the described radar. The answer is considered correct if the absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
0 0 1
6 0 3

```




```input2
-10 10 3
10 -10 3

```




```output1
1.000000000000000
```




```output2
11.142135623730951
```



## Note

<p>The figure below shows the answer to the first sample. In this sample the best decision is to put the radar at point with coordinates <span class="tex-span">(2, 0)</span>. </p><center> <img class="tex-graphics" src="file://h9x9FPYo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The figure below shows the answer for the second sample. In this sample the best decision is to put the radar at point with coordinates <span class="tex-span">(0, 0)</span>. </p><center> <img class="tex-graphics" src="file://3A8aJTZf.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
