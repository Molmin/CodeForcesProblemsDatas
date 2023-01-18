## Description

<div><p>As you very well know, the whole Universe traditionally uses three-dimensional Cartesian system of coordinates. In this system each point corresponds to three real coordinates <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span>. In this coordinate system, the distance between the center of the Universe and the point is calculated by the following formula: <img align="middle" class="tex-formula" src="file://yzeQxyOs.png" style="max-width: 100.0%;max-height: 100.0%;">. Mushroom scientists that work for the Great Mushroom King think that the Universe isn't exactly right and the distance from the center of the Universe to a point equals <span class="tex-span"><i>x</i><sup class="upper-index"><i>a</i></sup>·<i>y</i><sup class="upper-index"><i>b</i></sup>·<i>z</i><sup class="upper-index"><i>c</i></sup></span>.</p><p>To test the metric of mushroom scientists, the usual scientists offered them a task: find such <span class="tex-span"><i>x</i>, <i>y</i>, <i>z</i></span> <span class="tex-span">(0 ≤ <i>x</i>, <i>y</i>, <i>z</i>;&nbsp;<i>x</i> + <i>y</i> + <i>z</i> ≤ <i>S</i>)</span>, that the distance between the center of the Universe and the point <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span> is maximum possible in the metric of mushroom scientists. The mushroom scientists aren't good at maths, so they commissioned you to do the task.</p><p>Note that in this problem, it is considered that <span class="tex-span">0<sup class="upper-index">0</sup> = 1</span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>S</i></span> <span class="tex-span">(1 ≤ <i>S</i> ≤ 10<sup class="upper-index">3</sup>)</span> — the maximum sum of coordinates of the sought point.</p><p>The second line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> <span class="tex-span">(0 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">3</sup>)</span> — the numbers that describe the metric of mushroom scientists.</p></div><div class="output-specification"><p>Print three real numbers — the coordinates of the point that reaches maximum value in the metrics of mushroom scientists. If there are multiple answers, print any of them that meets the limitations.</p><p>A natural logarithm of distance from the center of the Universe to the given point in the metric of mushroom scientists shouldn't differ from the natural logarithm of the maximum distance by more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. We think that <span class="tex-span"><i>ln</i>(0) =  - ∞</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>S</i></span> <span class="tex-span">(1 ≤ <i>S</i> ≤ 10<sup class="upper-index">3</sup>)</span> — the maximum sum of coordinates of the sought point.</p><p>The second line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> <span class="tex-span">(0 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">3</sup>)</span> — the numbers that describe the metric of mushroom scientists.</p>

## Output

<p>Print three real numbers — the coordinates of the point that reaches maximum value in the metrics of mushroom scientists. If there are multiple answers, print any of them that meets the limitations.</p><p>A natural logarithm of distance from the center of the Universe to the given point in the metric of mushroom scientists shouldn't differ from the natural logarithm of the maximum distance by more than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. We think that <span class="tex-span"><i>ln</i>(0) =  - ∞</span>.</p>





```input1
3
1 1 1

```




```input2
3
2 0 0

```




```output1
1.0 1.0 1.0

```




```output2
3.0 0.0 0.0

```


