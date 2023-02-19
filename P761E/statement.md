## Description

<div><p>Dasha decided to have a rest after solving the problem. She had been ready to start her favourite activity — origami, but remembered the puzzle that she could not solve. </p><center> <img class="tex-graphics" src="file://wGNCTZJq.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The tree is a non-oriented connected graph without cycles. In particular, there always are <span class="tex-span"><i>n</i> - 1</span> edges in a tree with <span class="tex-span"><i>n</i></span> vertices.</p><p>The puzzle is to position the vertices at the points of the Cartesian plane with integral coordinates, so that the segments between the vertices connected by edges are parallel to the coordinate axes. Also, the intersection of segments is allowed only at their ends. Distinct vertices should be placed at different points. </p><p>Help Dasha to find any suitable way to position the tree vertices on the plane.</p><p>It is guaranteed that if it is possible to position the tree vertices on the plane without violating the condition which is given above, then you can do it by using points with integral coordinates which don't exceed <span class="tex-span">10<sup class="upper-index">18</sup></span> in absolute value.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 30)</span> — the number of vertices in the tree. </p><p>Each of next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) that mean that the <span class="tex-span"><i>i</i></span>-th edge of the tree connects vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the described graph is a tree.</p></div><div class="output-specification"><p>If the puzzle doesn't have a solution then in the only line print "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise, the first line should contain "<span class="tex-font-style-tt">YES</span>". The next <span class="tex-span"><i>n</i></span> lines should contain the pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">18</sup>)</span> — the coordinates of the point which corresponds to the <span class="tex-span"><i>i</i></span>-th vertex of the tree.</p><p>If there are several solutions, print any of them. </p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 30)</span> — the number of vertices in the tree. </p><p>Each of next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) that mean that the <span class="tex-span"><i>i</i></span>-th edge of the tree connects vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the described graph is a tree.</p>

## Output

<p>If the puzzle doesn't have a solution then in the only line print "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise, the first line should contain "<span class="tex-font-style-tt">YES</span>". The next <span class="tex-span"><i>n</i></span> lines should contain the pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">18</sup>)</span> — the coordinates of the point which corresponds to the <span class="tex-span"><i>i</i></span>-th vertex of the tree.</p><p>If there are several solutions, print any of them. </p>





```input1
7
1 2
1 3
2 4
2 5
3 6
3 7
```




```input2
6
1 2
2 3
2 4
2 5
2 6

```




```input3
4
1 2
2 3
3 4
```




```output1
YES
0 0
1 0
0 1
2 0
1 -1
-1 1
0 2
```




```output2
NO

```




```output3
YES
3 3
4 3
5 3
6 3
```



## Note

<p>In the first sample one of the possible positions of tree is: <img class="tex-graphics" src="file://aG7wdctS.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
