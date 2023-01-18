## Description

<div><p>An <span class="tex-font-style-it">oriented weighted forest</span> is an acyclic weighted digraph in which from each vertex at most one edge goes.</p><p>The <span class="tex-font-style-it">root</span> of vertex <span class="tex-span"><i>v</i></span> of an oriented weighted forest is a vertex from which no edge goes and which can be reached from vertex <span class="tex-span"><i>v</i></span> moving along the edges of the weighted oriented forest. We denote the root of vertex <span class="tex-span"><i>v</i></span> as <span class="tex-span"><i>root</i>(<i>v</i>)</span>.</p><p>The <span class="tex-font-style-it">depth</span> of vertex <span class="tex-span"><i>v</i></span> is the sum of weights of paths passing from the vertex <span class="tex-span"><i>v</i></span> to its root. Let's denote the depth of the vertex <span class="tex-span"><i>v</i></span> as <span class="tex-span"><i>depth</i>(<i>v</i>)</span>.</p><p>Let's consider the process of constructing a weighted directed forest. Initially, the forest does not contain vertices. Vertices are added sequentially one by one. Overall, there are <span class="tex-span"><i>n</i></span> performed operations of adding. The <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(<i>i</i> &gt; 0)</span> adding operation is described by a set of numbers <span class="tex-span">(<i>k</i>,  <i>v</i><sub class="lower-index">1</sub>,  <i>x</i><sub class="lower-index">1</sub>,  <i>v</i><sub class="lower-index">2</sub>,  <i>x</i><sub class="lower-index">2</sub>,  ... ,  <i>v</i><sub class="lower-index"><i>k</i></sub>,  <i>x</i><sub class="lower-index"><i>k</i></sub>)</span> and means that we should add vertex number <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>k</i></span> edges to the graph: an edge from vertex <span class="tex-span"><i>root</i>(<i>v</i><sub class="lower-index">1</sub>)</span> to vertex <span class="tex-span"><i>i</i></span> with weight <span class="tex-span"><i>depth</i>(<i>v</i><sub class="lower-index">1</sub>) + <i>x</i><sub class="lower-index">1</sub></span>, an edge from vertex <span class="tex-span"><i>root</i>(<i>v</i><sub class="lower-index">2</sub>)</span> to vertex <span class="tex-span"><i>i</i></span> with weight <span class="tex-span"><i>depth</i>(<i>v</i><sub class="lower-index">2</sub>) + <i>x</i><sub class="lower-index">2</sub></span> and so on. If <span class="tex-span"><i>k</i> = 0</span>, then only vertex <span class="tex-span"><i>i</i></span> is added to the graph, there are no added edges.</p><p>Your task is like this: given the operations of adding vertices, calculate the sum of the weights of all edges of the forest, resulting after the application of all defined operations, modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of operations of adding a vertex.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain descriptions of the operations, the <span class="tex-span"><i>i</i></span>-th line contains the description of the operation of adding the <span class="tex-span"><i>i</i></span>-th vertex in the following format: the first number of a line is an integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ <i>i</i> - 1)</span>, then follow <span class="tex-span">2<i>k</i></span> space-separated integers: <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">2</sub>, ... , <i>v</i><sub class="lower-index"><i>k</i></sub>, <i>x</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>j</i></sub> ≤ <i>i</i> - 1, |<i>x</i><sub class="lower-index"><i>j</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>. </p><p>The operations are given in the order, in which they should be applied to the graph. It is guaranteed that sum <span class="tex-span"><i>k</i></span> of all operations does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>, also that applying operations of adding vertexes does not result in loops and multiple edges. </p></div><div class="output-specification"><p>Print a single number — the sum of weights of all edges of the resulting graph modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of operations of adding a vertex.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain descriptions of the operations, the <span class="tex-span"><i>i</i></span>-th line contains the description of the operation of adding the <span class="tex-span"><i>i</i></span>-th vertex in the following format: the first number of a line is an integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ <i>i</i> - 1)</span>, then follow <span class="tex-span">2<i>k</i></span> space-separated integers: <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">2</sub>, ... , <i>v</i><sub class="lower-index"><i>k</i></sub>, <i>x</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>j</i></sub> ≤ <i>i</i> - 1, |<i>x</i><sub class="lower-index"><i>j</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>. </p><p>The operations are given in the order, in which they should be applied to the graph. It is guaranteed that sum <span class="tex-span"><i>k</i></span> of all operations does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>, also that applying operations of adding vertexes does not result in loops and multiple edges. </p>

## Output

<p>Print a single number — the sum of weights of all edges of the resulting graph modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
6
0
0
1 2 1
2 1 5 2 2
1 1 2
1 3 4

```




```input2
5
0
1 1 5
0
0
2 3 1 4 3

```




```output1
30

```




```output2
9

```



## Note

<p>Conside the first sample:</p><ol><li> Vertex <span class="tex-span">1</span> is added. <span class="tex-span"><i>k</i> = 0</span>, thus no edges are added.</li><li> Vertex <span class="tex-span">2</span> is added. <span class="tex-span"><i>k</i> = 0</span>, thus no edges are added.</li><li> Vertex <span class="tex-span">3</span> is added. <span class="tex-span"><i>k</i> = 1</span>. <span class="tex-span"><i>v</i><sub class="lower-index">1</sub> = 2</span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = 1</span>. Edge from vertex <span class="tex-span"><i>root</i>(2) = 2</span> to vertex <span class="tex-span">3</span> with weight <span class="tex-span"><i>depth</i>(2) + <i>x</i><sub class="lower-index">1</sub> = 0 + 1 = 1</span> is added. </li><li> Vertex <span class="tex-span">4</span> is added. <span class="tex-span"><i>k</i> = 2</span>. <span class="tex-span"><i>v</i><sub class="lower-index">1</sub> = 1</span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = 5</span>. Edge from vertex <span class="tex-span"><i>root</i>(1) = 1</span> to vertex <span class="tex-span">4</span> with weight <span class="tex-span"><i>depth</i>(1) + <i>x</i><sub class="lower-index">1</sub> = 0 + 5 = 5</span> is added. <span class="tex-span"><i>v</i><sub class="lower-index">2</sub> = 2</span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> = 2</span>. Edge from vertex <span class="tex-span"><i>root</i>(2) = 3</span> to vertex <span class="tex-span">4</span> with weight <span class="tex-span"><i>depth</i>(2) + <i>x</i><sub class="lower-index">1</sub> = 1 + 2 = 3</span> is added.</li><li> Vertex <span class="tex-span">5</span> is added. <span class="tex-span"><i>k</i> = 1</span>. <span class="tex-span"><i>v</i><sub class="lower-index">1</sub> = 1</span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = 2</span>. Edge from vertex <span class="tex-span"><i>root</i>(1) = 4</span> to vertex <span class="tex-span">5</span> with weight <span class="tex-span"><i>depth</i>(1) + <i>x</i><sub class="lower-index">1</sub> = 5 + 2 = 7</span> is added.</li><li> Vertex <span class="tex-span">6</span> is added. <span class="tex-span"><i>k</i> = 1</span>. <span class="tex-span"><i>v</i><sub class="lower-index">1</sub> = 3</span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = 4</span>. Edge from vertex <span class="tex-span"><i>root</i>(3) = 5</span> to vertex <span class="tex-span">6</span> with weight <span class="tex-span"><i>depth</i>(3) + <i>x</i><sub class="lower-index">1</sub> = 10 + 4 = 14</span> is added.</li></ol><p>The resulting graph is shown on the pictore below: <img class="tex-graphics" src="file://p0bIWmgN.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
