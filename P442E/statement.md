## Description

<div><p>Gena doesn't like geometry, so he asks you to solve this problem for him.</p><p>A rectangle with sides parallel to coordinate axes contains <span class="tex-span"><i>n</i></span> dots. Let's consider some point of the plane. Let's count the distances from this point to the given <span class="tex-span"><i>n</i></span> points. Let's sort these numbers in the non-decreasing order. We'll call the beauty of the point the second element of this array. If there are two mimimum elements in this array, the beaty will be equal to this minimum.</p><p>Find the maximum beauty of a point inside the given rectangle.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>w</i>, <i>h</i>, <i>n</i></span> (<span class="tex-span">1 ≤ <i>w</i>, <i>h</i> ≤ 10<sup class="upper-index">6</sup>, 2 ≤ <i>n</i> ≤ 1000</span>) — the lengths of the rectangle sides and the number of points. Next <span class="tex-span"><i>n</i></span> lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>w</i>, 0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i></span>) each — the coordinates of a point. It is possible that it will be coincident points.</p></div><div class="output-specification"><p>Print a single number — the maximum beauty of a point with the absolute or relative error of at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>w</i>, <i>h</i>, <i>n</i></span> (<span class="tex-span">1 ≤ <i>w</i>, <i>h</i> ≤ 10<sup class="upper-index">6</sup>, 2 ≤ <i>n</i> ≤ 1000</span>) — the lengths of the rectangle sides and the number of points. Next <span class="tex-span"><i>n</i></span> lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>w</i>, 0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i></span>) each — the coordinates of a point. It is possible that it will be coincident points.</p>

## Output

<p>Print a single number — the maximum beauty of a point with the absolute or relative error of at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
5 5 4
0 0
5 0
0 5
5 5

```




```input2
5 5 3
4 0
2 5
4 1

```




```output1
4.99999999941792340

```




```output2
5.65685424744772010

```



## Note

<p>The point which beauty we need to find must have coordinates (<span class="tex-span"><i>x</i>, <i>y</i></span>), where <span class="tex-span">0 ≤ <i>x</i> ≤ <i>w</i>, 0 ≤ <i>y</i> ≤ <i>h</i></span>. Some of the <span class="tex-span"><i>n</i></span> points can coincide.</p>
