## Description

<div><p>You are given a rectangle grid. That grid's size is <span class="tex-span"><i>n</i> × <i>m</i></span>. Let's denote the coordinate system on the grid. So, each point on the grid will have coordinates — a pair of integers <span class="tex-span">(<i>x</i>, <i>y</i>)</span> <span class="tex-span">(0 ≤ <i>x</i> ≤ <i>n</i>, 0 ≤ <i>y</i> ≤ <i>m</i>)</span>.</p><p>Your task is to find a maximum sub-rectangle on the grid <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> so that it contains the given point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, and its length-width ratio is exactly <span class="tex-span">(<i>a</i>, <i>b</i>)</span>. In other words the following conditions must hold: <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>, <img align="middle" class="tex-formula" src="file://qo59zoPb.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The sides of this sub-rectangle should be parallel to the axes. And values <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> should be integers.</p><center> <img class="tex-graphics" src="file://rj6LpfMb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>If there are multiple solutions, find the rectangle which is closest to <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. Here "closest" means the Euclid distance between <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and the center of the rectangle is as small as possible. If there are still multiple solutions, find the lexicographically minimum one. Here "lexicographically minimum" means that we should consider the sub-rectangle as sequence of integers <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, so we can choose the lexicographically minimum one.</p></div><div class="input-specification"><p>The first line contains six integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>x</i>, <i>y</i>, <i>a</i>, <i>b</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>x</i> ≤ <i>n</i>, 0 ≤ <i>y</i> ≤ <i>m</i>, 1 ≤ <i>a</i> ≤ <i>n</i>, 1 ≤ <i>b</i> ≤ <i>m</i>)</span>.</p></div><div class="output-specification"><p>Print four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>, which represent the founded sub-rectangle whose left-bottom point is <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and right-up point is <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p></div>

## Input

<p>The first line contains six integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>x</i>, <i>y</i>, <i>a</i>, <i>b</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>x</i> ≤ <i>n</i>, 0 ≤ <i>y</i> ≤ <i>m</i>, 1 ≤ <i>a</i> ≤ <i>n</i>, 1 ≤ <i>b</i> ≤ <i>m</i>)</span>.</p>

## Output

<p>Print four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>, which represent the founded sub-rectangle whose left-bottom point is <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and right-up point is <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p>





```input1
9 9 5 5 2 1

```




```input2
100 100 52 50 46 56

```




```output1
1 3 9 7

```




```output2
17 8 86 92

```


