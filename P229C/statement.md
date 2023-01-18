## Description

<div><p>Alice and Bob don't play games anymore. Now they study properties of all sorts of graphs together. Alice invented the following task: she takes a complete undirected graph with <span class="tex-span"><i>n</i></span> vertices, chooses some <span class="tex-span"><i>m</i></span> edges and keeps them. Bob gets the <img align="middle" class="tex-formula" src="file://3QKS1JIe.png" style="max-width: 100.0%;max-height: 100.0%;"> remaining edges.</p><p>Alice and Bob are fond of "triangles" in graphs, that is, cycles of length 3. That's why they wonder: what total number of triangles is there in the two graphs formed by Alice and Bob's edges, correspondingly?</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of vertices in the initial complete graph and the number of edges in Alice's graph, correspondingly. Then <span class="tex-span"><i>m</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), — the numbers of the two vertices connected by the <span class="tex-span"><i>i</i></span>-th edge in Alice's graph. It is guaranteed that Alice's graph contains no multiple edges and self-loops. It is guaranteed that the initial complete graph also contains no multiple edges and self-loops.</p><p>Consider the graph vertices to be indexed in some way from 1 to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Print a single number — the total number of cycles of length 3 in Alice and Bob's graphs together.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is advised to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of vertices in the initial complete graph and the number of edges in Alice's graph, correspondingly. Then <span class="tex-span"><i>m</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), — the numbers of the two vertices connected by the <span class="tex-span"><i>i</i></span>-th edge in Alice's graph. It is guaranteed that Alice's graph contains no multiple edges and self-loops. It is guaranteed that the initial complete graph also contains no multiple edges and self-loops.</p><p>Consider the graph vertices to be indexed in some way from 1 to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Print a single number — the total number of cycles of length 3 in Alice and Bob's graphs together.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is advised to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5 5
1 2
1 3
2 3
2 4
3 4

```




```input2
5 3
1 2
2 3
1 3

```




```output1
3

```




```output2
4

```



## Note

<p>In the first sample Alice has 2 triangles: (1, 2, 3) and (2, 3, 4). Bob's graph has only 1 triangle : (1, 4, 5). That's why the two graphs in total contain 3 triangles.</p><p>In the second sample Alice's graph has only one triangle: (1, 2, 3). Bob's graph has three triangles: (1, 4, 5), (2, 4, 5) and (3, 4, 5). In this case the answer to the problem is 4.</p>
