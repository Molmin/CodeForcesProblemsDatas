## Description

<div><p>You've got another geometrical task. You are given two non-degenerate polygons <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> as vertex coordinates. Polygon <span class="tex-span"><i>A</i></span> is strictly convex. Polygon <span class="tex-span"><i>B</i></span> is an arbitrary polygon without any self-intersections and self-touches. The vertices of both polygons are given in the clockwise order. For each polygon no three consecutively following vertices are located on the same straight line.</p><p>Your task is to check whether polygon <span class="tex-span"><i>B</i></span> is positioned strictly inside polygon <span class="tex-span"><i>A</i></span>. It means that any point of polygon <span class="tex-span"><i>B</i></span> should be strictly inside polygon <span class="tex-span"><i>A</i></span>. "Strictly" means that the vertex of polygon <span class="tex-span"><i>B</i></span> cannot lie on the side of the polygon <span class="tex-span"><i>A</i></span>.</p></div><div class="input-specification"><p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of vertices of polygon <span class="tex-span"><i>A</i></span>. Then <span class="tex-span"><i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>) — coordinates of the <span class="tex-span"><i>i</i></span>-th vertex of polygon <span class="tex-span"><i>A</i></span>. The vertices are given in the clockwise order.</p><p>The next line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">4</sup></span>) — the number of vertices of polygon <span class="tex-span"><i>B</i></span>. Then following <span class="tex-span"><i>m</i></span> lines contain pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>j</i></sub>|, |<i>y</i><sub class="lower-index"><i>j</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the <span class="tex-span"><i>j</i></span>-th vertex of polygon <span class="tex-span"><i>B</i></span>. The vertices are given in the clockwise order.</p><p>The coordinates of the polygon's vertices are separated by a single space. It is guaranteed that polygons <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> are non-degenerate, that polygon <span class="tex-span"><i>A</i></span> is strictly convex, that polygon <span class="tex-span"><i>B</i></span> has no self-intersections and self-touches and also for each polygon no three consecutively following vertices are located on the same straight line.</p></div><div class="output-specification"><p>Print on the only line the answer to the problem — if polygon <span class="tex-span"><i>B</i></span> is strictly inside polygon <span class="tex-span"><i>A</i></span>, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of vertices of polygon <span class="tex-span"><i>A</i></span>. Then <span class="tex-span"><i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>) — coordinates of the <span class="tex-span"><i>i</i></span>-th vertex of polygon <span class="tex-span"><i>A</i></span>. The vertices are given in the clockwise order.</p><p>The next line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">4</sup></span>) — the number of vertices of polygon <span class="tex-span"><i>B</i></span>. Then following <span class="tex-span"><i>m</i></span> lines contain pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>j</i></sub>|, |<i>y</i><sub class="lower-index"><i>j</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the <span class="tex-span"><i>j</i></span>-th vertex of polygon <span class="tex-span"><i>B</i></span>. The vertices are given in the clockwise order.</p><p>The coordinates of the polygon's vertices are separated by a single space. It is guaranteed that polygons <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> are non-degenerate, that polygon <span class="tex-span"><i>A</i></span> is strictly convex, that polygon <span class="tex-span"><i>B</i></span> has no self-intersections and self-touches and also for each polygon no three consecutively following vertices are located on the same straight line.</p>

## Output

<p>Print on the only line the answer to the problem — if polygon <span class="tex-span"><i>B</i></span> is strictly inside polygon <span class="tex-span"><i>A</i></span>, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
6
-2 1
0 3
3 3
4 1
3 -2
2 -2
4
0 1
2 2
3 1
1 0

```




```input2
5
1 2
4 2
3 -3
-2 -2
-2 1
4
0 1
1 2
4 1
2 -1

```




```input3
5
-1 2
2 3
4 1
3 -2
0 -3
5
1 0
1 1
3 1
5 -1
2 -1

```




```output1
YES

```




```output2
NO

```




```output3
NO

```


