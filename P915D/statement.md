## Description

<div><p>You are given a <a href="https://en.wikipedia.org/wiki/Directed_graph">directed graph</a> consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges (each edge is directed, so it can be traversed in only one direction). You are allowed to remove at most one edge from it.</p><p>Can you make this graph <a href="https://en.wikipedia.org/wiki/Directed_acyclic_graph">acyclic</a> by removing at most one edge from it? A directed graph is called acyclic iff it doesn't contain any cycle (a non-empty path that starts and ends in the same vertex).</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>min</i>(<i>n</i>(<i>n</i> - 1), 100000)</span>) — the number of vertices and the number of edges, respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow. Each line contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> denoting a directed edge going from vertex <span class="tex-span"><i>u</i></span> to vertex <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>). Each ordered pair <span class="tex-span">(<i>u</i>, <i>v</i>)</span> is listed at most once (there is at most one directed edge from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span>).</p></div><div class="output-specification"><p>If it is possible to make this graph acyclic by removing at most one edge, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>min</i>(<i>n</i>(<i>n</i> - 1), 100000)</span>) — the number of vertices and the number of edges, respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow. Each line contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> denoting a directed edge going from vertex <span class="tex-span"><i>u</i></span> to vertex <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>). Each ordered pair <span class="tex-span">(<i>u</i>, <i>v</i>)</span> is listed at most once (there is at most one directed edge from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span>).</p>

## Output

<p>If it is possible to make this graph acyclic by removing at most one edge, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
3 4
1 2
2 3
3 2
3 1

```




```input2
5 6
1 2
2 3
3 2
3 1
2 1
4 5

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first example you can remove edge <img align="middle" class="tex-formula" src="file://QBinzUkW.png" style="max-width: 100.0%;max-height: 100.0%;">, and the graph becomes acyclic.</p><p>In the second example you have to remove at least two edges (for example, <img align="middle" class="tex-formula" src="file://cWMu0f8v.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://NZwUM2Ed.png" style="max-width: 100.0%;max-height: 100.0%;">) in order to make the graph acyclic.</p>
