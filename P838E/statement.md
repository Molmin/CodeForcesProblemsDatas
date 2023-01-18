## Description

<div><p>You are given an strictly convex polygon with <span class="tex-span"><i>n</i></span> vertices. It is guaranteed that no three points are collinear. You would like to take a maximum non intersecting path on the polygon vertices that visits each point at most once.</p><p>More specifically your path can be represented as some sequence of distinct polygon vertices. Your path is the straight line segments between adjacent vertices in order. These segments are not allowed to touch or intersect each other except at the vertices in your sequence.</p><p>Given the polygon, print the maximum length non-intersecting path that visits each point at most once.</p></div><div class="input-specification"><p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2 500</span>), the number of points.</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>), denoting the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex.</p><p>It is guaranteed that these points are listed in clockwise order.</p></div><div class="output-specification"><p>Print a single floating point number, representing the longest non-intersecting path that visits the vertices at most once.</p><p>Your answer will be accepted if it has absolute or relative error at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>. More specifically, if your answer is <span class="tex-span"><i>a</i></span> and the jury answer is <span class="tex-span"><i>b</i></span>, your answer will be accepted if <img align="middle" class="tex-formula" src="file://DrOetqzF.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2 500</span>), the number of points.</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>), denoting the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex.</p><p>It is guaranteed that these points are listed in clockwise order.</p>

## Output

<p>Print a single floating point number, representing the longest non-intersecting path that visits the vertices at most once.</p><p>Your answer will be accepted if it has absolute or relative error at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>. More specifically, if your answer is <span class="tex-span"><i>a</i></span> and the jury answer is <span class="tex-span"><i>b</i></span>, your answer will be accepted if <img align="middle" class="tex-formula" src="file://DrOetqzF.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4
0 0
0 1
1 1
1 0

```




```output1
3.4142135624

```



## Note

<p>One optimal path is to visit points 0,1,3,2 in order.</p>
