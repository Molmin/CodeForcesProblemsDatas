## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> rectangles. The corners of rectangles have integer coordinates and their edges are parallel to the <span class="tex-span"><i>Ox</i></span> and <span class="tex-span"><i>Oy</i></span> axes. The rectangles may touch each other, but they do not overlap (that is, there are no points that belong to the interior of more than one rectangle). </p><p>Your task is to determine if the rectangles form a square. In other words, determine if the set of points inside or on the border of at least one rectangle is precisely equal to the set of points inside or on the border of some square.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5</span>). Next <span class="tex-span"><i>n</i></span> lines contain four integers each, describing a single rectangle: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 31400, 0 ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> ≤ 31400</span>) — <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> are <span class="tex-span"><i>x</i></span>-coordinates of the left and right edges of the rectangle, and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> are <span class="tex-span"><i>y</i></span>-coordinates of the bottom and top edges of the rectangle. </p><p>No two rectangles overlap (that is, there are no points that belong to the interior of more than one rectangle).</p></div><div class="output-specification"><p>In a single line print "<span class="tex-font-style-tt">YES</span>", if the given rectangles form a square, or "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5</span>). Next <span class="tex-span"><i>n</i></span> lines contain four integers each, describing a single rectangle: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> ≤ 31400, 0 ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> ≤ 31400</span>) — <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> are <span class="tex-span"><i>x</i></span>-coordinates of the left and right edges of the rectangle, and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> are <span class="tex-span"><i>y</i></span>-coordinates of the bottom and top edges of the rectangle. </p><p>No two rectangles overlap (that is, there are no points that belong to the interior of more than one rectangle).</p>

## Output

<p>In a single line print "<span class="tex-font-style-tt">YES</span>", if the given rectangles form a square, or "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
5
0 0 2 3
0 3 3 5
2 0 5 2
3 2 5 5
2 2 3 3

```




```input2
4
0 0 2 3
0 3 3 5
2 0 5 2
3 2 5 5

```




```output1
YES

```




```output2
NO

```


