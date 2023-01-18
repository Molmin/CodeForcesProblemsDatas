## Description

<div><p>You are given a connected weighted undirected graph without any loops and multiple edges. </p><p>Let us remind you that a graph's <span class="tex-font-style-underline">spanning tree</span> is defined as an acyclic connected subgraph of the given graph that includes all of the graph's vertexes. The <span class="tex-font-style-underline">weight</span> of a tree is defined as the sum of weights of the edges that the given tree contains. The <span class="tex-font-style-underline">minimum spanning tree</span> (<span class="tex-font-style-bf">MST</span>) of a graph is defined as the graph's spanning tree having the minimum possible weight. For any connected graph obviously exists the minimum spanning tree, but in the general case, a graph's minimum spanning tree is not unique.</p><p>Your task is to determine the following for each edge of the given graph: whether it is either included in <span class="tex-font-style-bf">any</span> MST, or included <span class="tex-font-style-bf">at least in one</span> MST, or <span class="tex-font-style-bf">not included in any</span> MST.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <img align="middle" class="tex-formula" src="file://XloxT5uR.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of the graph's vertexes and edges, correspondingly. Then follow <span class="tex-span"><i>m</i></span> lines, each of them contains three integers — the description of the graph's edges as "<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of vertexes connected by the <span class="tex-span"><i>i</i></span>-th edge, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is the edge's weight. It is guaranteed that the graph is connected and doesn't contain loops or multiple edges.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines — the answers for all edges. If the <span class="tex-span"><i>i</i></span>-th edge is included in any MST, print "<span class="tex-font-style-tt">any</span>"; if the <span class="tex-span"><i>i</i></span>-th edge is included at least in one MST, print "<span class="tex-font-style-tt">at least one</span>"; if the <span class="tex-span"><i>i</i></span>-th edge isn't included in any MST, print "<span class="tex-font-style-tt">none</span>". Print the answers for the edges in the order in which the edges are specified in the input.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <img align="middle" class="tex-formula" src="file://XloxT5uR.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of the graph's vertexes and edges, correspondingly. Then follow <span class="tex-span"><i>m</i></span> lines, each of them contains three integers — the description of the graph's edges as "<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of vertexes connected by the <span class="tex-span"><i>i</i></span>-th edge, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is the edge's weight. It is guaranteed that the graph is connected and doesn't contain loops or multiple edges.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines — the answers for all edges. If the <span class="tex-span"><i>i</i></span>-th edge is included in any MST, print "<span class="tex-font-style-tt">any</span>"; if the <span class="tex-span"><i>i</i></span>-th edge is included at least in one MST, print "<span class="tex-font-style-tt">at least one</span>"; if the <span class="tex-span"><i>i</i></span>-th edge isn't included in any MST, print "<span class="tex-font-style-tt">none</span>". Print the answers for the edges in the order in which the edges are specified in the input.</p>





```input1
4 5
1 2 101
1 3 100
2 3 2
2 4 2
3 4 1

```




```input2
3 3
1 2 1
2 3 1
1 3 2

```




```input3
3 3
1 2 1
2 3 1
1 3 1

```




```output1
none
any
at least one
at least one
any

```




```output2
any
any
none

```




```output3
at least one
at least one
at least one

```



## Note

<p>In the second sample the MST is unique for the given graph: it contains two first edges.</p><p>In the third sample any two edges form the MST for the given graph. That means that each edge is included at least in one MST.</p>
