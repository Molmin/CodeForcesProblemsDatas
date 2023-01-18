## Description

<div><p>You are given a rectangular grid of lattice points from <span class="tex-span">(0, 0)</span> to <span class="tex-span">(<i>n</i>, <i>m</i>)</span> inclusive. You have to choose exactly 4 different points to build a polyline possibly with self-intersections and self-touching. This polyline should be as long as possible.</p><p>A polyline defined by points <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub></span> consists of the line segments <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">2</sub> <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">3</sub> <i>p</i><sub class="lower-index">4</sub></span>, and its length is the sum of the lengths of the individual line segments.</p></div><div class="input-specification"><p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>n</i>, <i>m</i> ≤ 1000)</span>. It is guaranteed that grid contains at least 4 different points.</p></div><div class="output-specification"><p>Print 4 lines with two integers per line separated by space — coordinates of points <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub></span> in order which represent the longest possible polyline.</p><p>Judge program compares your answer and jury's answer with <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> precision.</p></div>

## Input

<p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>n</i>, <i>m</i> ≤ 1000)</span>. It is guaranteed that grid contains at least 4 different points.</p>

## Output

<p>Print 4 lines with two integers per line separated by space — coordinates of points <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub></span> in order which represent the longest possible polyline.</p><p>Judge program compares your answer and jury's answer with <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> precision.</p>





```input1
1 1

```




```input2
0 10

```




```output1
1 1
0 0
1 0
0 1

```




```output2
0 1
0 10
0 0
0 9

```


