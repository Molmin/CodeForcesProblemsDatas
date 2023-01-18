## Description

<div><p><span class="tex-font-style-it">Note the unusual memory limit for this problem.</span></p><p>You are given an undirected graph consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. The vertices are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, the edges are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Each edge can be unpainted or be painted in one of the <span class="tex-span"><i>k</i></span> colors, which are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>. Initially, none of the edges is painted in any of the colors.</p><p>You get queries of the form "Repaint edge <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span> to color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>". At any time the graph formed by the edges of the same color must be bipartite. If after the repaint this condition is violated, then the query is considered to be invalid and edge <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span> keeps its color. Otherwise, edge <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span> is repainted in color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, and the query is considered to valid.</p><p>Recall that the graph is called <span class="tex-font-style-it">bipartite</span> if the set of its vertices can be divided into two parts so that no edge connected vertices of the same parts.</p><p>For example, suppose you are given a triangle graph, that is a graph with three vertices and edges <span class="tex-span">(1, 2)</span>, <span class="tex-span">(2, 3)</span> and <span class="tex-span">(3, 1)</span>. Suppose that the first two edges are painted color <span class="tex-span">1</span>, and the third one is painted color <span class="tex-span">2</span>. Then the query of "repaint the third edge in color <span class="tex-span">1</span>" will be incorrect because after its execution the graph formed by the edges of color <span class="tex-span">1</span> will not be bipartite. On the other hand, it is possible to repaint the second edge in color <span class="tex-span">2</span>.</p><p>You receive <span class="tex-span"><i>q</i></span> queries. For each query, you should either apply it, and report that the query is valid, or report that the query is invalid.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i>, <i>q</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 50</span>) — the number of vertices, the number of edges, the number of colors and the number of queries. </p><p>Then follow <span class="tex-span"><i>m</i></span> edges of the graph in the form <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). </p><p>Then follow <span class="tex-span"><i>q</i></span> queries of the form <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>e</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>).</p><p>It is guaranteed that the graph doesn't contain multiple edges and loops.</p></div><div class="output-specification"><p>For each query print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if it is valid, or "<span class="tex-font-style-tt">NO</span>" (without the quotes), if this query destroys the bipartivity of the graph formed by the edges of some color.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i>, <i>q</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 50</span>) — the number of vertices, the number of edges, the number of colors and the number of queries. </p><p>Then follow <span class="tex-span"><i>m</i></span> edges of the graph in the form <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). </p><p>Then follow <span class="tex-span"><i>q</i></span> queries of the form <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>e</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>).</p><p>It is guaranteed that the graph doesn't contain multiple edges and loops.</p>

## Output

<p>For each query print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if it is valid, or "<span class="tex-font-style-tt">NO</span>" (without the quotes), if this query destroys the bipartivity of the graph formed by the edges of some color.</p>





```input1
3 3 2 5
1 2
2 3
1 3
1 1
2 1
3 2
3 1
2 2

```




```output1
YES
YES
YES
NO
YES

```


