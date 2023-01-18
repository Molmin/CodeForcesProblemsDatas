## Description

<div><p>There are <span class="tex-span"><i>n</i></span> points marked on the plane. The points are situated in such a way that they form a regular polygon (marked points are its vertices, and they are numbered in counter-clockwise order). You can draw <span class="tex-span"><i>n</i> - 1</span> segments, each connecting any two marked points, in such a way that all points have to be connected with each other (directly or indirectly).</p><p>But there are some restrictions. Firstly, some pairs of points cannot be connected directly and have to be connected undirectly. Secondly, the segments you draw must not intersect in any point apart from the marked points (that is, if any two segments intersect and their intersection is not a marked point, then the picture you have drawn is invalid).</p><p>How many ways are there to connect all vertices with <span class="tex-span"><i>n</i> - 1</span> segments? Two ways are considered different iff there exist some pair of points such that a segment is drawn between them in the first way of connection, but it is not drawn between these points in the second one. Since the answer might be large, output it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains one number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 500</span>) — the number of marked points.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each containing <span class="tex-span"><i>n</i></span> elements. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span"><i>j</i></span>-th element of line <span class="tex-span"><i>i</i></span>) is equal to <span class="tex-span">1</span> iff you can connect points <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> directly (otherwise <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>). It is guaranteed that for any pair of points <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>a</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span>, and for any point <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0</span>.</p></div><div class="output-specification"><p>Print the number of ways to connect points modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains one number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 500</span>) — the number of marked points.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each containing <span class="tex-span"><i>n</i></span> elements. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span"><i>j</i></span>-th element of line <span class="tex-span"><i>i</i></span>) is equal to <span class="tex-span">1</span> iff you can connect points <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> directly (otherwise <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>). It is guaranteed that for any pair of points <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>a</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span>, and for any point <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0</span>.</p>

## Output

<p>Print the number of ways to connect points modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3
0 0 1
0 0 1
1 1 0

```




```input2
4
0 1 1 1
1 0 1 1
1 1 0 1
1 1 1 0

```




```input3
3
0 0 0
0 0 1
0 1 0

```




```output1
1

```




```output2
12

```




```output3
0

```


