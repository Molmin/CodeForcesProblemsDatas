## Description

<div><p>John Doe has a field, which is a rectangular table of size <span class="tex-span"><i>n</i> × <i>m</i></span>. We assume that the field rows are numbered from 1 to <span class="tex-span"><i>n</i></span> from top to bottom, and the field columns are numbered from 1 to <span class="tex-span"><i>m</i></span> from left to right. Then the cell of the field at the intersection of the <span class="tex-span"><i>x</i></span>-th row and the <span class="tex-span"><i>y</i></span>-th column has coordinates (<span class="tex-span"><i>x</i></span>; <span class="tex-span"><i>y</i></span>).</p><p>We know that some cells of John's field are painted white, and some are painted black. Also, John has a tortoise, which can move along the white cells of the field. The tortoise can get from a white cell with coordinates (<span class="tex-span"><i>x</i></span>; <span class="tex-span"><i>y</i></span>) into cell (<span class="tex-span"><i>x</i> + 1</span>; <span class="tex-span"><i>y</i></span>) or (<span class="tex-span"><i>x</i></span>; <span class="tex-span"><i>y</i> + 1</span>), if the corresponding cell is painted white. In other words, the turtle can move only along the white cells of the field to the right or down. The turtle can not go out of the bounds of the field.</p><p>In addition, John has <span class="tex-span"><i>q</i></span> queries, each of them is characterized by four numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub></span>). For each query John wants to know whether the tortoise can start from the point with coordinates (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>), and reach the point with coordinates (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>), moving only along the white squares of the field.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>) — the field sizes.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters "<span class="tex-font-style-tt">#</span>" and "<span class="tex-font-style-tt">.</span>": the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals "<span class="tex-font-style-tt">#</span>", if the cell (<span class="tex-span"><i>i</i></span>; <span class="tex-span"><i>j</i></span>) is painted black and "<span class="tex-font-style-tt">.</span>", if it is painted white.</p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 6·10<sup class="upper-index">5</sup>)</span> — the number of queries. Next <span class="tex-span"><i>q</i></span> lines contain four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>) — the coordinates of the starting and the finishing cells. It is guaranteed that cells (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) and (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>) are white.</p></div><div class="output-specification"><p>For each of <span class="tex-span"><i>q</i></span> queries print on a single line "<span class="tex-font-style-tt">Yes</span>", if there is a way from cell (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) to cell (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>), that meets the requirements, and "<span class="tex-font-style-tt">No</span>" otherwise. Print the answers to the queries in the order, in which the queries are given in the input.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>) — the field sizes.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters "<span class="tex-font-style-tt">#</span>" and "<span class="tex-font-style-tt">.</span>": the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals "<span class="tex-font-style-tt">#</span>", if the cell (<span class="tex-span"><i>i</i></span>; <span class="tex-span"><i>j</i></span>) is painted black and "<span class="tex-font-style-tt">.</span>", if it is painted white.</p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 6·10<sup class="upper-index">5</sup>)</span> — the number of queries. Next <span class="tex-span"><i>q</i></span> lines contain four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>) — the coordinates of the starting and the finishing cells. It is guaranteed that cells (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) and (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>) are white.</p>

## Output

<p>For each of <span class="tex-span"><i>q</i></span> queries print on a single line "<span class="tex-font-style-tt">Yes</span>", if there is a way from cell (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) to cell (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>; <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>), that meets the requirements, and "<span class="tex-font-style-tt">No</span>" otherwise. Print the answers to the queries in the order, in which the queries are given in the input.</p>





```input1
3 3
...
.##
.#.
5
1 1 3 3
1 1 1 3
1 1 3 1
1 1 1 2
1 1 2 1

```




```input2
5 5
.....
.###.
.....
.###.
.....
5
1 1 5 5
1 1 1 5
1 1 3 4
2 1 2 5
1 1 2 5

```




```output1
No
Yes
Yes
Yes
Yes

```




```output2
Yes
Yes
Yes
No
Yes

```


