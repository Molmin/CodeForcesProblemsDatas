## Description

<div><p>John Doe decided that some mathematical object must be named after him. So he invented the Doe graphs. The Doe graphs are a family of undirected graphs, each of them is characterized by a single non-negative number — its order. </p><p>We'll denote a graph of order <span class="tex-span"><i>k</i></span> as <span class="tex-span"><i>D</i>(<i>k</i>)</span>, and we'll denote the number of vertices in the graph <span class="tex-span"><i>D</i>(<i>k</i>)</span> as <span class="tex-span">|<i>D</i>(<i>k</i>)|</span>. Then let's define the Doe graphs as follows:</p><ul> <li> <span class="tex-span"><i>D</i>(0)</span> consists of a single vertex, that has number <span class="tex-span">1</span>. </li><li> <span class="tex-span"><i>D</i>(1)</span> consists of two vertices with numbers <span class="tex-span">1</span> and <span class="tex-span">2</span>, connected by an edge. </li><li> <span class="tex-span"><i>D</i>(<i>n</i>)</span> for <span class="tex-span"><i>n</i> ≥ 2</span> is obtained from graphs <span class="tex-span"><i>D</i>(<i>n</i> - 1)</span> and <span class="tex-span"><i>D</i>(<i>n</i> - 2)</span>. <span class="tex-span"><i>D</i>(<i>n</i> - 1)</span> and <span class="tex-span"><i>D</i>(<i>n</i> - 2)</span> are joined in one graph, at that numbers of all vertices of graph <span class="tex-span"><i>D</i>(<i>n</i> - 2)</span> increase by <span class="tex-span">|<i>D</i>(<i>n</i> - 1)|</span> (for example, vertex number <span class="tex-span">1</span> of graph <span class="tex-span"><i>D</i>(<i>n</i> - 2)</span> becomes vertex number <span class="tex-span">1 + |<i>D</i>(<i>n</i> - 1)|</span>). After that two edges are added to the graph: the first one goes between vertices with numbers <span class="tex-span">|<i>D</i>(<i>n</i> - 1)|</span> and <span class="tex-span">|<i>D</i>(<i>n</i> - 1)| + 1</span>, the second one goes between vertices with numbers <span class="tex-span">|<i>D</i>(<i>n</i> - 1)| + 1</span> and <span class="tex-span">1</span>. Note that the definition of graph <span class="tex-span"><i>D</i>(<i>n</i>)</span> implies, that <span class="tex-span"><i>D</i>(<i>n</i>)</span> is a connected graph, its vertices are numbered from <span class="tex-span">1</span> to <span class="tex-span">|<i>D</i>(<i>n</i>)|</span>. </li></ul><center> <img class="tex-graphics" src="file://alSDG02o.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script">The picture shows the Doe graphs of order 1, 2, 3 and 4, from left to right.</span> </center><p>John thinks that Doe graphs are that great because for them exists a polynomial algorithm for the search of Hamiltonian path. However, your task is to answer queries of finding the shortest-length path between the vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> in the graph <span class="tex-span"><i>D</i>(<i>n</i>)</span>.</p><p>A path between a pair of vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> in the graph is a sequence of vertices <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(<i>k</i> &gt; 1)</span> such, that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>u</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub> = <i>v</i></span>, and for any <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>i</i> &lt; <i>k</i>)</span> vertices <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i> + 1</sub></span> are connected by a graph edge. The length of path <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span> is number <span class="tex-span">(<i>k</i> - 1)</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>) — the number of queries and the order of the given graph. The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">16</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — numbers of two vertices in the <span class="tex-span"><i>i</i></span>-th query. It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>D</i>(<i>n</i>)|</span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p></div><div class="output-specification"><p>For each query print a single integer on a single line — the length of the shortest path between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Print the answers to the queries in the order, in which the queries are given in the input.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>) — the number of queries and the order of the given graph. The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">16</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — numbers of two vertices in the <span class="tex-span"><i>i</i></span>-th query. It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>D</i>(<i>n</i>)|</span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p>

## Output

<p>For each query print a single integer on a single line — the length of the shortest path between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Print the answers to the queries in the order, in which the queries are given in the input.</p>





```input1
10 5
1 2
1 3
1 4
1 5
2 3
2 4
2 5
3 4
3 5
4 5

```




```output1
1
1
1
2
1
2
3
1
2
1

```


