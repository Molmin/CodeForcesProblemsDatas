## Description

<div><p>Bob likes to draw camels: with a single hump, two humps, three humps, etc. He draws a camel by connecting points on a coordinate plane. Now he's drawing camels with <span class="tex-span"><i>t</i></span> humps, representing them as polylines in the plane. Each polyline consists of <span class="tex-span"><i>n</i></span> vertices with coordinates <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>, <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, ..., <span class="tex-span">(<i>x</i><sub class="lower-index"><i>n</i></sub>, <i>y</i><sub class="lower-index"><i>n</i></sub>)</span>. The first vertex has a coordinate <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = 1</span>, the second — <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> = 2</span>, etc. Coordinates <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> might be any, but should satisfy the following conditions:</p><ul> <li> there should be <span class="tex-span"><i>t</i></span> humps precisely, i.e. such indexes <span class="tex-span"><i>j</i></span> (<span class="tex-span">2 ≤ <i>j</i> ≤ <i>n</i> - 1</span>), so that <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i> - 1</sub> &lt; <i>y</i><sub class="lower-index"><i>j</i></sub> &gt; <i>y</i><sub class="lower-index"><i>j</i> + 1</sub></span>, </li><li> there should be precisely <span class="tex-span"><i>t</i> - 1</span> such indexes <span class="tex-span"><i>j</i></span> (<span class="tex-span">2 ≤ <i>j</i> ≤ <i>n</i> - 1</span>), so that <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i> - 1</sub> &gt; <i>y</i><sub class="lower-index"><i>j</i></sub> &lt; <i>y</i><sub class="lower-index"><i>j</i> + 1</sub></span>, </li><li> no segment of a polyline should be parallel to the <span class="tex-span"><i>Ox</i></span>-axis, </li><li> all <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are integers between 1 and 4. </li></ul><p>For a series of his drawings of camels with <span class="tex-span"><i>t</i></span> humps Bob wants to buy a notebook, but he doesn't know how many pages he will need. Output the amount of different polylines that can be drawn to represent camels with <span class="tex-span"><i>t</i></span> humps for a given number <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The first line contains a pair of integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 20</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10</span>).</p></div><div class="output-specification"><p>Output the required amount of camels with <span class="tex-span"><i>t</i></span> humps.</p></div>

## Input

<p>The first line contains a pair of integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 20</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10</span>).</p>

## Output

<p>Output the required amount of camels with <span class="tex-span"><i>t</i></span> humps.</p>





```input1
6 1

```




```input2
4 2

```




```output1
6

```




```output2
0

```



## Note

<p>In the first sample test sequences of <span class="tex-span"><i>y</i></span>-coordinates for six camels are: 123421, 123431, 123432, 124321, 134321 и 234321 (each digit corresponds to one value of <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>).</p>
