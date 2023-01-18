## Description

<div><p>A connected undirected graph is called a <span class="tex-font-style-underline">vertex cactus</span>, if each vertex of this graph belongs to at most one simple cycle.</p><p>A <span class="tex-font-style-it">simple cycle</span> in a undirected graph is a sequence of distinct vertices <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>t</i></sub></span> <span class="tex-span">(<i>t</i> &gt; 2)</span>, such that for any <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>t</i>)</span> exists an edge between vertices <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span>, and also exists an edge between vertices <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>t</i></sub></span>.</p><p>A <span class="tex-font-style-it">simple path</span> in a undirected graph is a sequence of not necessarily distinct vertices <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>t</i></sub></span> <span class="tex-span">(<i>t</i> &gt; 0)</span>, such that for any <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>t</i>)</span> exists an edge between vertices <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> and furthermore each <span class="tex-font-style-bf">edge occurs no more than once</span>. We'll say that a simple path <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>t</i></sub></span> starts at vertex <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and ends at vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>t</i></sub></span>.</p><p>You've got a graph consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges, that is a vertex cactus. Also, you've got a list of <span class="tex-span"><i>k</i></span> pairs of interesting vertices <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span>, for which you want to know the following information — the number of distinct simple paths that start at vertex <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and end at vertex <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. We will consider two simple paths distinct if the sets of edges of the paths are distinct.</p><p>For each pair of interesting vertices count the number of distinct simple paths between them. As this number can be rather large, you should calculate it modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). </p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of vertices and edges in the graph, correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain the description of the edges: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the indexes of the vertices connected by the <span class="tex-span"><i>i</i></span>-th edge.</p><p>The next line contains a single integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of pairs of interesting vertices. Next <span class="tex-span"><i>k</i></span> lines contain the list of pairs of interesting vertices: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> — the indexes of interesting vertices in the <span class="tex-span"><i>i</i></span>-th pair.</p><p>It is guaranteed that the given graph is a vertex cactus. It is guaranteed that the graph contains no loops or multiple edges. Consider the graph vertices are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> lines: in the <span class="tex-span"><i>i</i></span>-th line print a single integer — the number of distinct simple ways, starting at <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and ending at <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of vertices and edges in the graph, correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain the description of the edges: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the indexes of the vertices connected by the <span class="tex-span"><i>i</i></span>-th edge.</p><p>The next line contains a single integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of pairs of interesting vertices. Next <span class="tex-span"><i>k</i></span> lines contain the list of pairs of interesting vertices: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> — the indexes of interesting vertices in the <span class="tex-span"><i>i</i></span>-th pair.</p><p>It is guaranteed that the given graph is a vertex cactus. It is guaranteed that the graph contains no loops or multiple edges. Consider the graph vertices are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Print <span class="tex-span"><i>k</i></span> lines: in the <span class="tex-span"><i>i</i></span>-th line print a single integer — the number of distinct simple ways, starting at <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and ending at <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
10 11
1 2
2 3
3 4
1 4
3 5
5 6
8 6
8 7
7 6
7 9
9 10
6
1 2
3 5
6 9
9 2
9 3
9 10

```




```output1
2
2
2
4
4
1

```


