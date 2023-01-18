## Description

<div><p>For a connected undirected weighted graph <span class="tex-span"><i>G</i></span>, MST (minimum spanning tree) is a subgraph of <span class="tex-span"><i>G</i></span> that contains all of <span class="tex-span"><i>G</i></span>'s vertices, is a tree, and sum of its edges is minimum possible.</p><p>You are given a graph <span class="tex-span"><i>G</i></span>. If you run a MST algorithm on graph it would give you only one MST and it causes other edges to become jealous. You are given some queries, each query contains a set of edges of graph <span class="tex-span"><i>G</i></span>, and you should determine whether there is a MST containing all these edges or not.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2  ≤ <i>n</i>, <i>m</i>  ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i></span>)&nbsp;— the number of vertices and edges in the graph and the number of queries.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the endpoints and weight of the <span class="tex-span"><i>i</i></span>-th edge. There can be more than one edges between two vertices. It's guaranteed that the given graph is connected.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries.</p><p><span class="tex-span"><i>q</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th of them contains the <span class="tex-span"><i>i</i></span>-th query. It starts with an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>)&nbsp;— the size of edges subset and continues with <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct space-separated integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>&nbsp;— the indices of the edges. It is guaranteed that the sum of <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> for <span class="tex-span">1 ≤ <i>i</i> ≤ <i>q</i></span> does not exceed <span class="tex-span">5·10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>For each query you should print "<span class="tex-font-style-tt">YES</span>" (without quotes) if there's a MST containing these edges and "<span class="tex-font-style-tt">NO</span>" (of course without quotes again) otherwise.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2  ≤ <i>n</i>, <i>m</i>  ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i></span>)&nbsp;— the number of vertices and edges in the graph and the number of queries.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the endpoints and weight of the <span class="tex-span"><i>i</i></span>-th edge. There can be more than one edges between two vertices. It's guaranteed that the given graph is connected.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries.</p><p><span class="tex-span"><i>q</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th of them contains the <span class="tex-span"><i>i</i></span>-th query. It starts with an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>)&nbsp;— the size of edges subset and continues with <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct space-separated integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>&nbsp;— the indices of the edges. It is guaranteed that the sum of <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> for <span class="tex-span">1 ≤ <i>i</i> ≤ <i>q</i></span> does not exceed <span class="tex-span">5·10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>For each query you should print "<span class="tex-font-style-tt">YES</span>" (without quotes) if there's a MST containing these edges and "<span class="tex-font-style-tt">NO</span>" (of course without quotes again) otherwise.</p>





```input1
5 7
1 2 2
1 3 2
2 3 1
2 4 1
3 4 1
3 5 2
4 5 2
4
2 3 4
3 3 4 5
2 1 7
2 1 2

```




```output1
YES
NO
YES
NO

```



## Note

<p>This is the graph of sample:</p><center> <img class="tex-graphics" height="302px" src="file://d0jNQOHK.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>Weight of minimum spanning tree on this graph is <span class="tex-span">6</span>.</p><p>MST with edges <span class="tex-span">(1, 3, 4, 6)</span>, contains all of edges from the first query, so answer on the first query is "<span class="tex-font-style-tt">YES</span>".</p><p>Edges from the second query form a cycle of length <span class="tex-span">3</span>, so there is no spanning tree including these three edges. Thus, answer is "<span class="tex-font-style-tt">NO</span>".</p>
