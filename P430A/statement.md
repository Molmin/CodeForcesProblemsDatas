## Description

<div><p>Iahub isn't well prepared on geometry problems, but he heard that this year there will be a lot of geometry problems on the IOI selection camp. Scared, Iahub locked himself in the basement and started thinking of new problems of this kind. One of them is the following.</p><p>Iahub wants to draw <span class="tex-span"><i>n</i></span> distinct points and <span class="tex-span"><i>m</i></span> segments on the <span class="tex-span"><i>OX</i></span> axis. He can draw each point with either red or blue. The drawing is good if and only if the following requirement is met: for each segment <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> consider all the red points belong to it (<span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> points), and all the blue points belong to it (<span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> points); each segment <span class="tex-span"><i>i</i></span> should satisfy the inequality <span class="tex-span">|<i>r</i><sub class="lower-index"><i>i</i></sub> - <i>b</i><sub class="lower-index"><i>i</i></sub>| ≤ 1</span>.</p><p>Iahub thinks that point <span class="tex-span"><i>x</i></span> belongs to segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>, if inequality <span class="tex-span"><i>l</i> ≤ <i>x</i> ≤ <i>r</i></span> holds.</p><p>Iahub gives to you all coordinates of points and segments. Please, help him to find any good drawing.</p></div><div class="input-specification"><p>The first line of input contains two integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>). The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the coordinates of the points. The following <span class="tex-span"><i>m</i></span> lines contain the descriptions of the <span class="tex-span"><i>m</i></span> segments. Each line contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the borders of the <span class="tex-span"><i>i</i></span>-th segment.</p><p>It's guaranteed that all the points are distinct.</p></div><div class="output-specification"><p>If there is no good drawing for a given test, output a single integer -1. Otherwise output <span class="tex-span"><i>n</i></span> integers, each integer must be 0 or 1. The <span class="tex-span"><i>i</i></span>-th number denotes the color of the <span class="tex-span"><i>i</i></span>-th point (0 is red, and 1 is blue).</p><p>If there are multiple good drawings you can output any of them.</p></div>

## Input

<p>The first line of input contains two integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>). The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the coordinates of the points. The following <span class="tex-span"><i>m</i></span> lines contain the descriptions of the <span class="tex-span"><i>m</i></span> segments. Each line contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the borders of the <span class="tex-span"><i>i</i></span>-th segment.</p><p>It's guaranteed that all the points are distinct.</p>

## Output

<p>If there is no good drawing for a given test, output a single integer -1. Otherwise output <span class="tex-span"><i>n</i></span> integers, each integer must be 0 or 1. The <span class="tex-span"><i>i</i></span>-th number denotes the color of the <span class="tex-span"><i>i</i></span>-th point (0 is red, and 1 is blue).</p><p>If there are multiple good drawings you can output any of them.</p>





```input1
3 3
3 7 14
1 5
6 10
11 15

```




```input2
3 4
1 2 3
1 2
2 3
5 6
2 2

```




```output1
0 0 0
```




```output2
1 0 1
```


