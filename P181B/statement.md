## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> points on a plane. All points are different.</p><p>Find the number of different groups of three points <span class="tex-span">(<i>A</i>, <i>B</i>, <i>C</i>)</span> such that point <span class="tex-span"><i>B</i></span> is the middle of segment <span class="tex-span"><i>AC</i></span>. </p><p>The groups of three points are considered unordered, that is, if point <span class="tex-span"><i>B</i></span> is the middle of segment <span class="tex-span"><i>AC</i></span>, then groups <span class="tex-span">(<i>A</i>, <i>B</i>, <i>C</i>)</span> and <span class="tex-span">(<i>C</i>, <i>B</i>, <i>A</i>)</span> are considered the same.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3000</span>) — the number of points. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain the points. The <span class="tex-span"><i>i</i></span>-th line contains coordinates of the <span class="tex-span"><i>i</i></span>-th point: two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p><p>It is guaranteed that all given points are different.</p></div><div class="output-specification"><p>Print the single number — the answer to the problem. </p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3000</span>) — the number of points. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain the points. The <span class="tex-span"><i>i</i></span>-th line contains coordinates of the <span class="tex-span"><i>i</i></span>-th point: two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p><p>It is guaranteed that all given points are different.</p>

## Output

<p>Print the single number — the answer to the problem. </p>





```input1
3
1 1
2 2
3 3

```




```input2
3
0 0
-1 0
0 1

```




```output1
1

```




```output2
0

```


