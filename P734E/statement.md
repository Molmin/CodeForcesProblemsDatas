## Description

<div><p>Anton is growing a tree in his garden. In case you forgot, the tree is a connected acyclic undirected graph.</p><p>There are <span class="tex-span"><i>n</i></span> vertices in the tree, each of them is painted black or white. Anton doesn't like multicolored trees, so he wants to change the tree such that all vertices have the same color (black or white).</p><p>To change the colors Anton can use only operations of one type. We denote it as <span class="tex-span"><i>paint</i>(<i>v</i>)</span>, where <span class="tex-span"><i>v</i></span> is some vertex of the tree. This operation changes the color of all vertices <span class="tex-span"><i>u</i></span> such that all vertices on the shortest path from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span> have the same color (including <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span>). For example, consider the tree</p><center> <img class="tex-graphics" src="file://yLE7SWCF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>and apply operation <span class="tex-span"><i>paint</i>(3)</span> to get the following:</p><center> <img class="tex-graphics" src="file://BLYtorHY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Anton is interested in the minimum number of operation he needs to perform in order to make the colors of all vertices equal.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>color</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>color</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>)&nbsp;— colors of the vertices. <span class="tex-span"><i>color</i><sub class="lower-index"><i>i</i></sub> = 0</span> means that the <span class="tex-span"><i>i</i></span>-th vertex is initially painted white, while <span class="tex-span"><i>color</i><sub class="lower-index"><i>i</i></sub> = 1</span> means it's initially painted black.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> line, each of them contains a pair of integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— indices of vertices connected by the corresponding edge. It's guaranteed that all pairs <span class="tex-span">(<i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>)</span> are distinct, i.e. there are no multiple edges.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum number of operations Anton has to apply in order to make all vertices of the tree black or all vertices of the tree white.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>color</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>color</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>)&nbsp;— colors of the vertices. <span class="tex-span"><i>color</i><sub class="lower-index"><i>i</i></sub> = 0</span> means that the <span class="tex-span"><i>i</i></span>-th vertex is initially painted white, while <span class="tex-span"><i>color</i><sub class="lower-index"><i>i</i></sub> = 1</span> means it's initially painted black.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> line, each of them contains a pair of integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— indices of vertices connected by the corresponding edge. It's guaranteed that all pairs <span class="tex-span">(<i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>)</span> are distinct, i.e. there are no multiple edges.</p>

## Output

<p>Print one integer&nbsp;— the minimum number of operations Anton has to apply in order to make all vertices of the tree black or all vertices of the tree white.</p>





```input1
11
0 0 0 1 1 0 1 0 0 1 1
1 2
1 3
2 4
2 5
5 6
5 7
3 8
3 9
3 10
9 11

```




```input2
4
0 0 0 0
1 2
2 3
3 4

```




```output1
2

```




```output2
0

```



## Note

<p>In the first sample, the tree is the same as on the picture. If we first apply operation <span class="tex-span"><i>paint</i>(3)</span> and then apply <span class="tex-span"><i>paint</i>(6)</span>, the tree will become completely black, so the answer is <span class="tex-span">2</span>.</p><p>In the second sample, the tree is already white, so there is no need to apply any operations and the answer is <span class="tex-span">0</span>.</p>
