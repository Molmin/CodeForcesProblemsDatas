## Description

<div><p>The Zoo in the Grid Kingdom is represented by an infinite grid. The Zoo has <span class="tex-span"><i>n</i></span> observation binoculars located at the <span class="tex-span"><i>OX</i></span> axis. For each <span class="tex-span"><i>i</i></span> between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>, inclusive, there exists a single binocular located at the point with coordinates <span class="tex-span">(<i>i</i>, 0)</span>. There are <span class="tex-span"><i>m</i></span> flamingos in the Zoo, located at points with positive coordinates. The flamingos are currently sleeping and you can assume that they don't move.</p><p>In order to get a good view over the flamingos, each of the binoculars can be independently rotated to face any angle (not necessarily integer). Then, the binocular can be used to observe all flamingos that is located at the straight line passing through the binocular at the angle it is set. In other words, you can assign each binocular a direction corresponding to any straight line passing through the binocular, and the binocular will be able to see all flamingos located on that line.</p><p>Today, some kids from the prestigious Codeforces kindergarten went on a Field Study to the Zoo. Their teacher would like to set each binocular an angle to maximize the number of flamingos that can be seen by the binocular. The teacher is very interested in the sum of these values over all binoculars. Please help him find this sum.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>m</i> ≤ 250)</span>, denoting the number of binoculars and the number of flamingos, respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th line will contain two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), which means that the <span class="tex-span"><i>i</i></span>-th flamingo is located at point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. </p><p>All flamingos will be located at distinct points.</p></div><div class="output-specification"><p>Print a single integer denoting the maximum total number of flamingos that can be seen by all the binoculars.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>m</i> ≤ 250)</span>, denoting the number of binoculars and the number of flamingos, respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th line will contain two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), which means that the <span class="tex-span"><i>i</i></span>-th flamingo is located at point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. </p><p>All flamingos will be located at distinct points.</p>

## Output

<p>Print a single integer denoting the maximum total number of flamingos that can be seen by all the binoculars.</p>





```input1
5 5
2 1
4 1
3 2
4 3
4 4

```




```output1
11

```



## Note

<p>This picture shows the answer to the example test case. </p><center> <img class="tex-graphics" src="file://a6co48g0.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
