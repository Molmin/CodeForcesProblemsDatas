## Description

<div><p>A set of points on a plane is called <span class="tex-font-style-underline">good</span>, if for any two points at least one of the three conditions is true:</p><ul><li> those two points lie on same horizontal line; </li><li> those two points lie on same vertical line; </li><li> the rectangle, with corners in these two points, contains inside or on its borders at least one point of the set, other than these two. We mean here a rectangle with sides parallel to coordinates' axes, the so-called bounding box of the two points.</li></ul><p>You are given a set consisting of <span class="tex-span"><i>n</i></span> points on a plane. Find any good superset of the given set whose size would not exceed <span class="tex-span">2·10<sup class="upper-index">5</sup></span> points.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of points in the initial set. Next <span class="tex-span"><i>n</i></span> lines describe the set's points. Each line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — a corresponding point's coordinates. It is guaranteed that all the points are different.</p></div><div class="output-specification"><p>Print on the first line the number of points <span class="tex-span"><i>m</i></span> (<span class="tex-span"><i>n</i> ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) in a good superset, print on next <span class="tex-span"><i>m</i></span> lines the points. The absolute value of the points' coordinates should not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. Note that you should not minimize <span class="tex-span"><i>m</i></span>, it is enough to find any good superset of the given set, whose size does not exceed <span class="tex-span">2·10<sup class="upper-index">5</sup></span>.</p><p>All points in the superset should have integer coordinates.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of points in the initial set. Next <span class="tex-span"><i>n</i></span> lines describe the set's points. Each line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — a corresponding point's coordinates. It is guaranteed that all the points are different.</p>

## Output

<p>Print on the first line the number of points <span class="tex-span"><i>m</i></span> (<span class="tex-span"><i>n</i> ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) in a good superset, print on next <span class="tex-span"><i>m</i></span> lines the points. The absolute value of the points' coordinates should not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. Note that you should not minimize <span class="tex-span"><i>m</i></span>, it is enough to find any good superset of the given set, whose size does not exceed <span class="tex-span">2·10<sup class="upper-index">5</sup></span>.</p><p>All points in the superset should have integer coordinates.</p>





```input1
2
1 1
2 2

```




```output1
3
1 1
2 2
1 2

```


