## Description

<div><p>You are given a multiset of points on the plane with integer coordinates. Find the maximum distance between two points from this multiset.</p></div><div class="input-specification"><p>The first line of input contains the number of points <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>). Next, <span class="tex-span"><i>n</i></span> pairs of lines follow, each describing a single point: the first line contains <span class="tex-span"><i>x</i></span>-coordinate, the second one — the <span class="tex-span"><i>y</i></span>-coordinate (<span class="tex-span"> - 50 ≤ <i>x</i>, <i>y</i> ≤ 50</span>). Some of the points can have identical coordinates.</p></div><div class="output-specification"><p>Output the maximum distance between two points from this multiset. The answer is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line of input contains the number of points <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>). Next, <span class="tex-span"><i>n</i></span> pairs of lines follow, each describing a single point: the first line contains <span class="tex-span"><i>x</i></span>-coordinate, the second one — the <span class="tex-span"><i>y</i></span>-coordinate (<span class="tex-span"> - 50 ≤ <i>x</i>, <i>y</i> ≤ 50</span>). Some of the points can have identical coordinates.</p>

## Output

<p>Output the maximum distance between two points from this multiset. The answer is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
3
0
1
2
3
4
5

```




```input2
3
10
12
-5
8
10
12

```




```output1
5.656854249

```




```output2
15.5241747

```



## Note

<p>In the first case the maximum distance is between points <span class="tex-span">(0, 1)</span> and <span class="tex-span">(4, 5)</span>. In the second case two of the points are the same, so the maximum distance is between one of them and the third point.</p>
