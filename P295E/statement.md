## Description

<div><p>Yaroslav has <span class="tex-span"><i>n</i></span> points that lie on the <span class="tex-span"><i>Ox</i></span> axis. The coordinate of the first point is <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, the coordinate of the second point is <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, ..., the coordinate of the <span class="tex-span"><i>n</i></span>-th point is — <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span>. Now Yaroslav wants to execute <span class="tex-span"><i>m</i></span> queries, each of them is of one of the two following types:</p><ol> <li> Move the <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span>-th point from position <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>j</i></sub></sub></span> to position <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>j</i></sub></sub> + <i>d</i><sub class="lower-index"><i>j</i></sub></span>. At that, it is guaranteed that after executing such query all coordinates of the points will be distinct. </li><li> Count the sum of distances between all pairs of points that lie on the segment <span class="tex-span">[<i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub>]</span> <span class="tex-span">(<i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub>)</span>. In other words, you should count the sum of: <img align="middle" class="tex-formula" src="file://xRw5H04X.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ol><p>Help Yaroslav.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of points <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> — the coordinates of points <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> — the number of queries <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next <span class="tex-span"><i>m</i></span> lines contain the queries. The <span class="tex-span"><i>j</i></span>-th line first contains integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ 2)</span> — the query type. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub> = 1</span>, then it is followed by two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, |<i>d</i><sub class="lower-index"><i>j</i></sub>| ≤ 1000)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub> = 2</span>, then it is followed by two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>It is guaranteed that at any moment all the points have distinct coordinates.</p></div><div class="output-specification"><p>For each type 2 query print the answer on a single line. Print the answers in the order, in which the queries follow in the input.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams of the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of points <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> — the coordinates of points <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> — the number of queries <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next <span class="tex-span"><i>m</i></span> lines contain the queries. The <span class="tex-span"><i>j</i></span>-th line first contains integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ 2)</span> — the query type. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub> = 1</span>, then it is followed by two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, |<i>d</i><sub class="lower-index"><i>j</i></sub>| ≤ 1000)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub> = 2</span>, then it is followed by two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>It is guaranteed that at any moment all the points have distinct coordinates.</p>

## Output

<p>For each type 2 query print the answer on a single line. Print the answers in the order, in which the queries follow in the input.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams of the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
8
36 50 28 -75 40 -60 -95 -48
20
2 -61 29
1 5 -53
1 1 429
1 5 130
2 -101 -71
2 -69 53
1 1 404
1 5 518
2 -101 53
2 50 872
1 1 -207
2 -99 -40
1 7 -389
1 6 -171
1 2 464
1 7 -707
1 1 -730
1 1 560
2 635 644
1 7 -677

```




```output1
176
20
406
1046
1638
156
0

```


