## Description

<div><p>Imagine an <span class="tex-span"><i>n</i> × <i>m</i></span> grid with some blocked cells. The top left cell in the grid has coordinates <span class="tex-span">(1, 1)</span> and the bottom right cell has coordinates <span class="tex-span">(<i>n</i>, <i>m</i>)</span>. There are <span class="tex-span"><i>k</i></span> blocked cells in the grid and others are empty. You flash a laser beam from the center of an empty cell <span class="tex-span">(<i>x</i><sub class="lower-index"><i>s</i></sub>, <i>y</i><sub class="lower-index"><i>s</i></sub>)</span> in one of the diagonal directions (i.e. north-east, north-west, south-east or south-west). If the beam hits a blocked cell or the border of the grid it will reflect. The behavior of the beam reflection in different situations is depicted in the figure below. </p><center> <img class="tex-graphics" src="file://7QMMN3g3.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>After a while the beam enters an infinite cycle. Count the number of empty cells that the beam goes through at least once. We consider that the beam goes through cell if it goes through its center.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Each of the next <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>)</span> indicating the position of the <span class="tex-span"><i>i</i></span>-th blocked cell. </p><p>The last line contains <span class="tex-span"><i>x</i><sub class="lower-index"><i>s</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>s</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>s</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>s</i></sub> ≤ <i>m</i>)</span> and the flash direction which is equal to "<span class="tex-font-style-tt">NE</span>", "<span class="tex-font-style-tt">NW</span>", "<span class="tex-font-style-tt">SE</span>" or "<span class="tex-font-style-tt">SW</span>". These strings denote directions <span class="tex-span">( - 1, 1)</span>, <span class="tex-span">( - 1,  - 1)</span>, <span class="tex-span">(1, 1)</span>, <span class="tex-span">(1,  - 1)</span>.</p><p>It's guaranteed that no two blocked cells have the same coordinates.</p></div><div class="output-specification"><p>In the only line of the output print the number of empty cells that the beam goes through at least once.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Each of the next <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>)</span> indicating the position of the <span class="tex-span"><i>i</i></span>-th blocked cell. </p><p>The last line contains <span class="tex-span"><i>x</i><sub class="lower-index"><i>s</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>s</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>s</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>s</i></sub> ≤ <i>m</i>)</span> and the flash direction which is equal to "<span class="tex-font-style-tt">NE</span>", "<span class="tex-font-style-tt">NW</span>", "<span class="tex-font-style-tt">SE</span>" or "<span class="tex-font-style-tt">SW</span>". These strings denote directions <span class="tex-span">( - 1, 1)</span>, <span class="tex-span">( - 1,  - 1)</span>, <span class="tex-span">(1, 1)</span>, <span class="tex-span">(1,  - 1)</span>.</p><p>It's guaranteed that no two blocked cells have the same coordinates.</p>

## Output

<p>In the only line of the output print the number of empty cells that the beam goes through at least once.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3 3 0
1 2 SW

```




```input2
7 5 3
3 3
4 3
5 3
2 1 SE

```




```output1
6

```




```output2
14

```


