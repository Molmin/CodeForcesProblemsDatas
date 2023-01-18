## Description

<div><p>Hongcow is ruler of the world. As ruler of the world, he wants to make it easier for people to travel by road within their own countries.</p><p>The world can be modeled as an undirected graph with <span class="tex-span"><i>n</i></span> nodes and <span class="tex-span"><i>m</i></span> edges. <span class="tex-span"><i>k</i></span> of the nodes are home to the governments of the <span class="tex-span"><i>k</i></span> countries that make up the world.</p><p>There is at most one edge connecting any two nodes and no edge connects a node to itself. Furthermore, for any two nodes corresponding to governments, <span class="tex-font-style-bf">there is no path between those two nodes</span>. Any graph that satisfies all of these conditions is <span class="tex-font-style-it">stable</span>.</p><p>Hongcow wants to add as many edges as possible to the graph while keeping it stable. Determine the maximum number of edges Hongcow can add.</p></div><div class="input-specification"><p>The first line of input will contain three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of vertices and edges in the graph, and the number of vertices that are homes of the government. </p><p>The next line of input will contain <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). These integers will be pairwise distinct and denote the nodes that are home to the governments in this world.</p><p>The following <span class="tex-span"><i>m</i></span> lines of input will contain two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). This denotes an undirected edge between nodes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the graph described by the input is stable.</p></div><div class="output-specification"><p>Output a single integer, the maximum number of edges Hongcow can add to the graph while keeping it stable.</p></div>

## Input

<p>The first line of input will contain three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of vertices and edges in the graph, and the number of vertices that are homes of the government. </p><p>The next line of input will contain <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). These integers will be pairwise distinct and denote the nodes that are home to the governments in this world.</p><p>The following <span class="tex-span"><i>m</i></span> lines of input will contain two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). This denotes an undirected edge between nodes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the graph described by the input is stable.</p>

## Output

<p>Output a single integer, the maximum number of edges Hongcow can add to the graph while keeping it stable.</p>





```input1
4 1 2
1 3
1 2

```




```input2
3 3 1
2
1 2
1 3
2 3

```




```output1
2

```




```output2
0

```



## Note

<p>For the first sample test, the graph looks like this: </p><center> <img class="tex-graphics" src="file://AFOjChTi.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> Vertices <span class="tex-span">1</span> and <span class="tex-span">3</span> are special. The optimal solution is to connect vertex <span class="tex-span">4</span> to vertices <span class="tex-span">1</span> and <span class="tex-span">2</span>. This adds a total of <span class="tex-span">2</span> edges. We cannot add any more edges, since vertices <span class="tex-span">1</span> and <span class="tex-span">3</span> cannot have any path between them.<p>For the second sample test, the graph looks like this: </p><center> <img class="tex-graphics" src="file://Vy7tAwdq.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> We cannot add any more edges to this graph. Note that we are not allowed to add self-loops, and the graph must be simple.
