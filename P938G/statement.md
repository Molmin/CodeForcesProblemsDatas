## Description

<div><p>You are given an undirected connected graph with weighted edges. The length of some path between two vertices is the bitwise xor of weights of all edges belonging to this path (if some edge is traversed more than once, then it is included in bitwise xor the same number of times). </p><p>There are three types of queries you have to process:</p><ul> <li> <span class="tex-span">1</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>d</i></span> — add an edge connecting vertex <span class="tex-span"><i>x</i></span> to vertex <span class="tex-span"><i>y</i></span> with weight <span class="tex-span"><i>d</i></span>. It is guaranteed that there is no edge connecting <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span> before this query; </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> — remove an edge connecting vertex <span class="tex-span"><i>x</i></span> to vertex <span class="tex-span"><i>y</i></span>. It is guaranteed that there was such edge in the graph, and the graph stays connected after this query; </li><li> <span class="tex-span">3</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> — calculate the length of the shortest path (possibly non-simple) from vertex <span class="tex-span"><i>x</i></span> to vertex <span class="tex-span"><i>y</i></span>. </li></ul><p>Print the answers for all queries of type <span class="tex-span">3</span>.</p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200000</span>) — the number of vertices and the number of edges in the graph, respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow denoting the edges of the graph. Each line contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>d</i> ≤ 2<sup class="upper-index">30</sup> - 1</span>). Each pair <span class="tex-span">(<i>x</i>, <i>y</i>)</span> is listed at most once. The initial graph is connected.</p><p>Then one line follows, containing an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200000</span>) — the number of queries you have to process.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, denoting queries in the following form:</p><ul> <li> <span class="tex-span">1</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>d</i> ≤ 2<sup class="upper-index">30</sup> - 1</span>) — add an edge connecting vertex <span class="tex-span"><i>x</i></span> to vertex <span class="tex-span"><i>y</i></span> with weight <span class="tex-span"><i>d</i></span>. It is guaranteed that there is no edge connecting <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span> before this query; </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>n</i></span>) — remove an edge connecting vertex <span class="tex-span"><i>x</i></span> to vertex <span class="tex-span"><i>y</i></span>. It is guaranteed that there was such edge in the graph, and the graph stays connected after this query; </li><li> <span class="tex-span">3</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>n</i></span>) — calculate the length of the shortest path (possibly non-simple) from vertex <span class="tex-span"><i>x</i></span> to vertex <span class="tex-span"><i>y</i></span>. </li></ul><p>It is guaranteed that at least one query has type <span class="tex-span">3</span>.</p></div><div class="output-specification"><p>Print the answers for all queries of type <span class="tex-span">3</span> in the order they appear in input.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200000</span>) — the number of vertices and the number of edges in the graph, respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow denoting the edges of the graph. Each line contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>d</i> ≤ 2<sup class="upper-index">30</sup> - 1</span>). Each pair <span class="tex-span">(<i>x</i>, <i>y</i>)</span> is listed at most once. The initial graph is connected.</p><p>Then one line follows, containing an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200000</span>) — the number of queries you have to process.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, denoting queries in the following form:</p><ul> <li> <span class="tex-span">1</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>d</i> ≤ 2<sup class="upper-index">30</sup> - 1</span>) — add an edge connecting vertex <span class="tex-span"><i>x</i></span> to vertex <span class="tex-span"><i>y</i></span> with weight <span class="tex-span"><i>d</i></span>. It is guaranteed that there is no edge connecting <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span> before this query; </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>n</i></span>) — remove an edge connecting vertex <span class="tex-span"><i>x</i></span> to vertex <span class="tex-span"><i>y</i></span>. It is guaranteed that there was such edge in the graph, and the graph stays connected after this query; </li><li> <span class="tex-span">3</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>n</i></span>) — calculate the length of the shortest path (possibly non-simple) from vertex <span class="tex-span"><i>x</i></span> to vertex <span class="tex-span"><i>y</i></span>. </li></ul><p>It is guaranteed that at least one query has type <span class="tex-span">3</span>.</p>

## Output

<p>Print the answers for all queries of type <span class="tex-span">3</span> in the order they appear in input.</p>





```input1
5 5
1 2 3
2 3 4
3 4 5
4 5 6
1 5 1
5
3 1 5
1 1 3 1
3 1 5
2 1 5
3 1 5

```




```output1
1
1
2

```


