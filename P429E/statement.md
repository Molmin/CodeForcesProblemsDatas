## Description

<div><p>Iahub isn't well prepared on geometry problems, but he heard that this year there will be a lot of geometry problems on the IOI selection camp. Scared, Iahub locked himself in the basement and started thinking of new problems of this kind. One of them is the following.</p><p>Iahub wants to draw <span class="tex-span"><i>n</i></span> distinct segments <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> on the <span class="tex-span"><i>OX</i></span> axis. He can draw each segment with either red or blue. The drawing is good if and only if the following requirement is met: for each point <span class="tex-span"><i>x</i></span> of the <span class="tex-span"><i>OX</i></span> axis consider all the segments that contains point <span class="tex-span"><i>x</i></span>; suppose, that <span class="tex-span"><i>r</i><sub class="lower-index"><i>x</i></sub></span> red segments and <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub></span> blue segments contain point <span class="tex-span"><i>x</i></span>; for each point <span class="tex-span"><i>x</i></span> inequality <span class="tex-span">|<i>r</i><sub class="lower-index"><i>x</i></sub> - <i>b</i><sub class="lower-index"><i>x</i></sub>| ≤ 1</span> must be satisfied.</p><p>A segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> contains a point <span class="tex-span"><i>x</i></span> if and only if <span class="tex-span"><i>l</i> ≤ <i>x</i> ≤ <i>r</i></span>.</p><p>Iahub gives you the starting and ending points of all the segments. You have to find any good drawing for him.</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of segments. The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the borders of the <span class="tex-span"><i>i</i></span>-th segment.</p><p>It's guaranteed that all the segments are distinct.</p></div><div class="output-specification"><p>If there is no good drawing for a given test, output a single integer -1. Otherwise output <span class="tex-span"><i>n</i></span> integers; each integer must be 0 or 1. The <span class="tex-span"><i>i</i></span>-th number denotes the color of the <span class="tex-span"><i>i</i></span>-th segment (0 is red and 1 is blue).</p><p>If there are multiple good drawings you can output any of them.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of segments. The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the borders of the <span class="tex-span"><i>i</i></span>-th segment.</p><p>It's guaranteed that all the segments are distinct.</p>

## Output

<p>If there is no good drawing for a given test, output a single integer -1. Otherwise output <span class="tex-span"><i>n</i></span> integers; each integer must be 0 or 1. The <span class="tex-span"><i>i</i></span>-th number denotes the color of the <span class="tex-span"><i>i</i></span>-th segment (0 is red and 1 is blue).</p><p>If there are multiple good drawings you can output any of them.</p>





```input1
2
0 2
2 3

```




```input2
6
1 5
1 3
3 5
2 10
11 11
12 12

```




```output1
0 1

```




```output2
0 1 0 1 0 0

```


