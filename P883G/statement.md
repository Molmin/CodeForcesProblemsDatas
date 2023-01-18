## Description

<div><p>Vasya has a graph containing both directed (oriented) and undirected (non-oriented) edges. There can be multiple edges between a pair of vertices.</p><p>Vasya has picked a vertex <span class="tex-span"><i>s</i></span> from the graph. Now Vasya wants to create two separate plans:</p><ol> <li> to orient each undirected edge in one of two possible directions to <span class="tex-font-style-it">maximize</span> number of vertices reachable from vertex <span class="tex-span"><i>s</i></span>; </li><li> to orient each undirected edge in one of two possible directions to <span class="tex-font-style-it">minimize</span> number of vertices reachable from vertex <span class="tex-span"><i>s</i></span>. </li></ol><p>In each of two plans each undirected edge must become directed. For an edge chosen directions can differ in two plans.</p><p>Help Vasya find the plans.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>) — number of vertices and edges in the graph, and the vertex Vasya has picked.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain information about the graph edges. Each line contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>) — edge type and vertices connected by the edge. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span> then the edge is directed and goes from the vertex <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to the vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span> then the edge is undirected and it connects the vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that there is at least one undirected edge in the graph.</p></div><div class="output-specification"><p>The first two lines should describe the plan which maximizes the number of reachable vertices. The lines three and four should describe the plan which minimizes the number of reachable vertices.</p><p>A description of each plan should start with a line containing the number of reachable vertices. The second line of a plan should consist of <span class="tex-span"><i>f</i></span> symbols '<span class="tex-font-style-tt">+</span>' and '<span class="tex-font-style-tt">-</span>', where <span class="tex-span"><i>f</i></span> is the number of undirected edges in the initial graph. Print '<span class="tex-font-style-tt">+</span>' as the <span class="tex-span"><i>j</i></span>-th symbol of the string if the <span class="tex-span"><i>j</i></span>-th undirected edge <span class="tex-span">(<i>u</i>, <i>v</i>)</span> from the input should be oriented from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span>. Print '<span class="tex-font-style-tt">-</span>' to signify the opposite direction (from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>). Consider undirected edges to be numbered in the same order they are given in the input.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>) — number of vertices and edges in the graph, and the vertex Vasya has picked.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain information about the graph edges. Each line contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>) — edge type and vertices connected by the edge. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span> then the edge is directed and goes from the vertex <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to the vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span> then the edge is undirected and it connects the vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that there is at least one undirected edge in the graph.</p>

## Output

<p>The first two lines should describe the plan which maximizes the number of reachable vertices. The lines three and four should describe the plan which minimizes the number of reachable vertices.</p><p>A description of each plan should start with a line containing the number of reachable vertices. The second line of a plan should consist of <span class="tex-span"><i>f</i></span> symbols '<span class="tex-font-style-tt">+</span>' and '<span class="tex-font-style-tt">-</span>', where <span class="tex-span"><i>f</i></span> is the number of undirected edges in the initial graph. Print '<span class="tex-font-style-tt">+</span>' as the <span class="tex-span"><i>j</i></span>-th symbol of the string if the <span class="tex-span"><i>j</i></span>-th undirected edge <span class="tex-span">(<i>u</i>, <i>v</i>)</span> from the input should be oriented from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span>. Print '<span class="tex-font-style-tt">-</span>' to signify the opposite direction (from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>). Consider undirected edges to be numbered in the same order they are given in the input.</p><p>If there are multiple solutions, print any of them.</p>





```input1
2 2 1
1 1 2
2 2 1

```




```input2
6 6 3
2 2 6
1 4 5
2 3 4
1 4 1
1 3 1
2 2 3

```




```output1
2
-
2
+

```




```output2
6
++-
2
+-+

```


