## Description

<div><p>Mr. Kitayuta has just bought an undirected graph consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. The vertices of the graph are numbered from 1 to <span class="tex-span"><i>n</i></span>. Each edge, namely edge <span class="tex-span"><i>i</i></span>, has a color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, connecting vertex <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Mr. Kitayuta wants you to process the following <span class="tex-span"><i>q</i></span> queries.</p><p>In the <span class="tex-span"><i>i</i></span>-th query, he gives you two integers — <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Find the number of the colors that satisfy the following condition: the edges of that color connect vertex <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> directly or indirectly.</p></div><div class="input-specification"><p>The first line of the input contains space-separated two integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100, 1 ≤ <i>m</i> ≤ 100</span>), denoting the number of the vertices and the number of the edges, respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain space-separated three integers — <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>). Note that there can be multiple edges between two vertices. However, there are no multiple edges of the same color between two vertices, that is, if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>, <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>) ≠ (<i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub>, <i>c</i><sub class="lower-index"><i>j</i></sub>)</span>.</p><p>The next line contains a integer — <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100</span>), denoting the number of the queries.</p><p>Then follows <span class="tex-span"><i>q</i></span> lines, containing space-separated two integers — <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). It is guaranteed that <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>For each query, print the answer in a separate line.</p></div>

## Input

<p>The first line of the input contains space-separated two integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100, 1 ≤ <i>m</i> ≤ 100</span>), denoting the number of the vertices and the number of the edges, respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain space-separated three integers — <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>). Note that there can be multiple edges between two vertices. However, there are no multiple edges of the same color between two vertices, that is, if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>, <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>) ≠ (<i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub>, <i>c</i><sub class="lower-index"><i>j</i></sub>)</span>.</p><p>The next line contains a integer — <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100</span>), denoting the number of the queries.</p><p>Then follows <span class="tex-span"><i>q</i></span> lines, containing space-separated two integers — <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). It is guaranteed that <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>For each query, print the answer in a separate line.</p>





```input1
4 5
1 2 1
1 2 2
2 3 1
2 3 3
2 4 3
3
1 2
3 4
1 4

```




```input2
5 7
1 5 1
2 5 1
3 5 1
4 5 1
1 2 2
2 3 2
3 4 2
5
1 5
5 1
2 5
1 5
1 4

```




```output1
2
1
0

```




```output2
1
1
1
1
2

```



## Note

<p>Let's consider the first sample. </p><center> <img class="tex-graphics" src="file://NUc2DhXk.png" style="max-width: 100.0%;max-height: 100.0%;">   The figure above shows the first sample. </center> <ul> <li> Vertex <span class="tex-span">1</span> and vertex <span class="tex-span">2</span> are connected by color <span class="tex-span">1</span> and <span class="tex-span">2</span>. </li><li> Vertex <span class="tex-span">3</span> and vertex <span class="tex-span">4</span> are connected by color <span class="tex-span">3</span>. </li><li> Vertex <span class="tex-span">1</span> and vertex <span class="tex-span">4</span> are not connected by any single color. </li></ul>
