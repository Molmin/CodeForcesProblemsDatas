## Description

<div><p>George loves graphs. Most of all, he loves interesting graphs. We will assume that a directed graph is <span class="tex-font-style-it">interesting</span>, if it meets the following criteria: </p><ul> <li> The graph doesn't contain any multiple arcs; </li><li> There is vertex <span class="tex-span"><i>v</i></span> (we'll call her the <span class="tex-font-style-it">center</span>), such that for any vertex of graph <span class="tex-span"><i>u</i></span>, the graph contains arcs <span class="tex-span">(<i>u</i>, <i>v</i>)</span> and <span class="tex-span">(<i>v</i>, <i>u</i>)</span>. Please note that the graph also contains loop <span class="tex-span">(<i>v</i>, <i>v</i>)</span>. </li><li> The outdegree of all vertexes except for the <span class="tex-font-style-it">center</span> equals two and the indegree of all vertexes except for the <span class="tex-font-style-it">center</span> equals two. The outdegree of vertex <span class="tex-span"><i>u</i></span> is the number of arcs that go out of <span class="tex-span"><i>u</i></span>, the indegree of vertex <span class="tex-span"><i>u</i></span> is the number of arcs that go in <span class="tex-span"><i>u</i></span>. Please note that the graph can contain loops. </li></ul><p>However, not everything's that simple. George got a directed graph of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> arcs as a present. The graph didn't have any multiple arcs. As George loves interesting graphs, he wants to slightly alter the presented graph and transform it into an interesting one. In one alteration he can either remove an arbitrary existing arc from the graph or add an arbitrary arc to the graph. </p><p>George wonders: what is the minimum number of changes that he needs to obtain an interesting graph from the graph he's got as a present? Help George and find the answer to the question.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500, 1 ≤ <i>m</i> ≤ 1000</span>) — the number of vertices and arcs in the presented graph.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the descriptions of the graph's arcs. Pair <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> means that the graph contains an arc from vertex number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to vertex number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that the presented graph doesn't contain multiple arcs.</p><p>Assume that the grah vertices are numbered 1 through <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Print a single integer — the answer to George's question.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500, 1 ≤ <i>m</i> ≤ 1000</span>) — the number of vertices and arcs in the presented graph.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the descriptions of the graph's arcs. Pair <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> means that the graph contains an arc from vertex number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to vertex number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that the presented graph doesn't contain multiple arcs.</p><p>Assume that the grah vertices are numbered 1 through <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Print a single integer — the answer to George's question.</p>





```input1
3 7
1 1
2 2
3 1
1 3
3 2
2 3
3 3

```




```input2
3 6
1 1
2 2
3 1
3 2
2 3
3 3

```




```input3
3 1
2 2

```




```output1
0

```




```output2
1

```




```output3
6

```



## Note

<p>For more information about directed graphs, please visit: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Directed_graph</span></p><p>In the first sample the graph already is interesting, its center is vertex <span class="tex-span">3</span>.</p>
