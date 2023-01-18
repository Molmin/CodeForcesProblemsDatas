## Description

<div><p>Meg the Rabbit decided to do something nice, specifically — to determine the shortest distance between two points on the surface of our planet. But Meg... what can you say, she wants everything simple. So, she already regards our planet as a two-dimensional circle. No, wait, it's even worse — as a square of side <span class="tex-span"><i>n</i></span>. Thus, the task has been reduced to finding the shortest path between two dots on a square (the path should go through the square sides). To simplify the task let us consider the vertices of the square to lie at points whose coordinates are: <span class="tex-span">(0, 0)</span>, <span class="tex-span">(<i>n</i>, 0)</span>, <span class="tex-span">(0, <i>n</i>)</span> and <span class="tex-span">(<i>n</i>, <i>n</i>)</span>.</p></div><div class="input-specification"><p>The single line contains 5 space-separated integers: <span class="tex-span"><i>n</i>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 0 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>) which correspondingly represent a side of the square, the coordinates of the first point and the coordinates of the second point. It is guaranteed that the points lie on the sides of the square.</p></div><div class="output-specification"><p>You must print on a single line the shortest distance between the points.</p></div>

## Input

<p>The single line contains 5 space-separated integers: <span class="tex-span"><i>n</i>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 0 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>) which correspondingly represent a side of the square, the coordinates of the first point and the coordinates of the second point. It is guaranteed that the points lie on the sides of the square.</p>

## Output

<p>You must print on a single line the shortest distance between the points.</p>





```input1
2 0 0 1 0

```




```input2
2 0 1 2 1

```




```input3
100 0 0 100 100

```




```output1
1

```




```output2
4

```




```output3
200

```


