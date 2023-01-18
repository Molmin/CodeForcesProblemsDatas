## Description

<div><p>There are <span class="tex-span"><i>n</i></span> points on a straight line, and the <span class="tex-span"><i>i</i></span>-th point among them is located at <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. All these coordinates are distinct.</p><p>Determine the number <span class="tex-span"><i>m</i></span> — the smallest number of points you should add on the line to make the distances between all neighboring points equal. </p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000</span>) — the number of points.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the points. All these coordinates are distinct. The points can be given in an arbitrary order.</p></div><div class="output-specification"><p>Print a single integer <span class="tex-span"><i>m</i></span> — the smallest number of points you should add on the line to make the distances between all neighboring points equal. </p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000</span>) — the number of points.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the points. All these coordinates are distinct. The points can be given in an arbitrary order.</p>

## Output

<p>Print a single integer <span class="tex-span"><i>m</i></span> — the smallest number of points you should add on the line to make the distances between all neighboring points equal. </p>





```input1
3
-5 10 5

```




```input2
6
100 200 400 300 600 500

```




```input3
4
10 9 0 -1

```




```output1
1

```




```output2
0

```




```output3
8

```



## Note

<p>In the first example you can add one point with coordinate <span class="tex-span">0</span>.</p><p>In the second example the distances between all neighboring points are already equal, so you shouldn't add anything.</p>
