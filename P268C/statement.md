## Description

<div><p>Manao has invented a new mathematical term — a beautiful set of points. He calls a set of points on a plane <span class="tex-font-style-it">beautiful</span> if it meets the following conditions:</p><ol> <li> The coordinates of each point in the set are integers. </li><li> For any two points from the set, the distance between them is a non-integer. </li></ol><p>Consider all points <span class="tex-span">(<i>x</i>, <i>y</i>)</span> which satisfy the inequations: <span class="tex-span">0 ≤ <i>x</i> ≤ <i>n</i></span>; <span class="tex-span">0 ≤ <i>y</i> ≤ <i>m</i></span>; <span class="tex-span"><i>x</i> + <i>y</i> &gt; 0</span>. Choose their subset of maximum size such that it is also a beautiful set of points.</p></div><div class="input-specification"><p>The single line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>).</p></div><div class="output-specification"><p>In the first line print a single integer — the size <span class="tex-span"><i>k</i></span> of the found beautiful set. In each of the next <span class="tex-span"><i>k</i></span> lines print a pair of space-separated integers — the <span class="tex-span"><i>x</i></span>- and <span class="tex-span"><i>y</i></span>- coordinates, respectively, of a point from the set.</p><p>If there are several optimal solutions, you may print any of them.</p></div>

## Input

<p>The single line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>).</p>

## Output

<p>In the first line print a single integer — the size <span class="tex-span"><i>k</i></span> of the found beautiful set. In each of the next <span class="tex-span"><i>k</i></span> lines print a pair of space-separated integers — the <span class="tex-span"><i>x</i></span>- and <span class="tex-span"><i>y</i></span>- coordinates, respectively, of a point from the set.</p><p>If there are several optimal solutions, you may print any of them.</p>





```input1
2 2

```




```input2
4 3

```




```output1
3
0 1
1 2
2 0

```




```output2
4
0 3
2 1
3 0
4 2

```



## Note

<p>Consider the first sample. The distance between points (0, 1) and (1, 2) equals <img align="middle" class="tex-formula" src="file://ZszgJ5lf.png" style="max-width: 100.0%;max-height: 100.0%;">, between (0, 1) and (2, 0) — <img align="middle" class="tex-formula" src="file://69AU1SQr.png" style="max-width: 100.0%;max-height: 100.0%;">, between (1, 2) and (2, 0) — <img align="middle" class="tex-formula" src="file://7kzTfrOa.png" style="max-width: 100.0%;max-height: 100.0%;">. Thus, these points form a beautiful set. You cannot form a beautiful set with more than three points out of the given points. Note that this is not the only solution.</p>
