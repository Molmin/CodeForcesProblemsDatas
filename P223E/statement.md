## Description

<div><p>A graph is called <span class="tex-font-style-it">planar</span>, if it can be drawn in such a way that its edges intersect only at their vertexes.</p><p>An <span class="tex-font-style-it">articulation point</span> is such a vertex of an undirected graph, that when removed increases the number of connected components of the graph.</p><p>A <span class="tex-font-style-it">bridge</span> is such an edge of an undirected graph, that when removed increases the number of connected components of the graph.</p><p>You've got a connected undirected planar graph consisting of <span class="tex-span"><i>n</i></span> vertexes, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, drawn on the plane. The graph has no bridges, articulation points, loops and multiple edges. You are also given <span class="tex-span"><i>q</i></span> queries. Each query is a cycle in the graph. The query response is the number of graph vertexes, which (if you draw a graph and the cycle on the plane) are located either inside the cycle, or on it. Write a program that, given the graph and the queries, will answer each query.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of vertexes and edges of the graph. Next <span class="tex-span"><i>m</i></span> lines contain the edges of the graph: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the numbers of vertexes, connecting the <span class="tex-span"><i>i</i></span>-th edge. The next <span class="tex-span"><i>n</i></span> lines contain the positions of the planar graph vertexes on the plane: the <span class="tex-span"><i>i</i></span>-th line contains a pair of space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex of the graph on the plane. </p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries. Then follow <span class="tex-span"><i>q</i></span> lines that describe the queries: the <span class="tex-span"><i>i</i></span>-th line contains the sequence of space-separated integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>;&nbsp;<i>k</i><sub class="lower-index"><i>i</i></sub> &gt; 2</span>), where <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> is the cycle length in the <span class="tex-span"><i>i</i></span>-th query, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> are numbers of the vertexes that form a cycle. The numbers of vertexes in the cycle are given in the clockwise or counterclockwise order. The given cycles are simple, that is they cannot go through a graph vertex more than once. The total length of all cycles in all queries does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>It is guaranteed that the given graph contains no bridges, articulation points, loops and multiple edges. It is guaranteed that the edge segments can have common points only at the graph's vertexes.</p></div><div class="output-specification"><p>For each query print a single integer — the number of vertexes inside the cycle or on it. Print the answers in the order, in which the queries follow in the input. Separate the numbers by spaces.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of vertexes and edges of the graph. Next <span class="tex-span"><i>m</i></span> lines contain the edges of the graph: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the numbers of vertexes, connecting the <span class="tex-span"><i>i</i></span>-th edge. The next <span class="tex-span"><i>n</i></span> lines contain the positions of the planar graph vertexes on the plane: the <span class="tex-span"><i>i</i></span>-th line contains a pair of space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex of the graph on the plane. </p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries. Then follow <span class="tex-span"><i>q</i></span> lines that describe the queries: the <span class="tex-span"><i>i</i></span>-th line contains the sequence of space-separated integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>;&nbsp;<i>k</i><sub class="lower-index"><i>i</i></sub> &gt; 2</span>), where <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> is the cycle length in the <span class="tex-span"><i>i</i></span>-th query, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> are numbers of the vertexes that form a cycle. The numbers of vertexes in the cycle are given in the clockwise or counterclockwise order. The given cycles are simple, that is they cannot go through a graph vertex more than once. The total length of all cycles in all queries does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>It is guaranteed that the given graph contains no bridges, articulation points, loops and multiple edges. It is guaranteed that the edge segments can have common points only at the graph's vertexes.</p>

## Output

<p>For each query print a single integer — the number of vertexes inside the cycle or on it. Print the answers in the order, in which the queries follow in the input. Separate the numbers by spaces.</p>





```input1
3 3
1 2
2 3
3 1
0 0
1 0
0 1
1
3 1 2 3

```




```input2
5 8
1 2
2 3
3 4
4 1
1 5
2 5
3 5
4 5
0 0
2 0
2 2
0 2
1 1
1
4 1 2 3 4

```




```input3
4 5
1 2
2 3
3 4
4 1
2 4
0 0
1 0
1 1
0 1
3
3 1 2 4
3 4 2 3
4 1 2 3 4

```




```output1
3

```




```output2
5

```




```output3
3
3
4

```


