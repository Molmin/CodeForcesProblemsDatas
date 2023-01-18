## Description

<div><p>Vika has an infinite sheet of squared paper. Initially all squares are white. She introduced a two-dimensional coordinate system on this sheet and drew <span class="tex-span"><i>n</i></span> black horizontal and vertical segments parallel to the coordinate axes. All segments have width equal to <span class="tex-span">1</span> square, that means every segment occupy some set of neighbouring squares situated in one row or one column.</p><p>Your task is to calculate the number of painted cells. If a cell was painted more than once, it should be calculated exactly once.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of segments drawn by Vika.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of the endpoints of the segments drawn by Vika. It is guaranteed that all the segments are parallel to coordinate axes. Segments may touch, overlap and even completely coincide.</p></div><div class="output-specification"><p>Print the number of cells painted by Vika. If a cell was painted more than once, it should be calculated exactly once in the answer.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of segments drawn by Vika.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of the endpoints of the segments drawn by Vika. It is guaranteed that all the segments are parallel to coordinate axes. Segments may touch, overlap and even completely coincide.</p>

## Output

<p>Print the number of cells painted by Vika. If a cell was painted more than once, it should be calculated exactly once in the answer.</p>





```input1
3
0 1 2 1
1 4 1 2
0 3 2 3

```




```input2
4
-2 -1 2 -1
2 1 -2 1
-1 -2 -1 2
1 2 1 -2

```




```output1
8

```




```output2
16

```



## Note

<p>In the first sample Vika will paint squares <span class="tex-span">(0, 1)</span>, <span class="tex-span">(1, 1)</span>, <span class="tex-span">(2, 1)</span>, <span class="tex-span">(1, 2)</span>, <span class="tex-span">(1, 3)</span>, <span class="tex-span">(1, 4)</span>, <span class="tex-span">(0, 3)</span> and <span class="tex-span">(2, 3)</span>.</p>
