## Description

<div><p>You are given a directed graph with <span class="tex-span"><i>n</i></span> nodes and <span class="tex-span"><i>m</i></span> edges, with all edges having a certain weight. </p><p>There might be multiple edges and self loops, and the graph can also be disconnected. </p><p>You need to choose a path (possibly passing through same vertices multiple times) in the graph such that the weights of the edges are in strictly increasing order, and these edges come in the order of input. Among all such paths, you need to find the the path that has the maximum possible number of edges, and report this value.</p><p>Please note that the edges picked don't have to be consecutive in the input.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>,<span class="tex-span">1 ≤ <i>m</i> ≤ 100000</span>)&nbsp;— the number of vertices and edges in the graph, respectively. </p><p><span class="tex-span"><i>m</i></span> lines follows. </p><p>The <span class="tex-span"><i>i</i></span>-th of these lines contains three space separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100000</span>), denoting an edge from vertex <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to vertex <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> having weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span></p></div><div class="output-specification"><p>Print one integer in a single line — the maximum number of edges in the path.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>,<span class="tex-span">1 ≤ <i>m</i> ≤ 100000</span>)&nbsp;— the number of vertices and edges in the graph, respectively. </p><p><span class="tex-span"><i>m</i></span> lines follows. </p><p>The <span class="tex-span"><i>i</i></span>-th of these lines contains three space separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100000</span>), denoting an edge from vertex <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to vertex <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> having weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span></p>

## Output

<p>Print one integer in a single line — the maximum number of edges in the path.</p>





```input1
3 3
3 1 3
1 2 1
2 3 2

```




```input2
5 5
1 3 2
3 2 3
3 4 5
5 4 0
4 5 8

```




```output1
2
```




```output2
3
```



## Note

<p>The answer for the first sample input is <span class="tex-span">2</span>: <img align="middle" class="tex-formula" src="file://kdbEPZMU.png" style="max-width: 100.0%;max-height: 100.0%;">. Note that you cannot traverse <img align="middle" class="tex-formula" src="file://1hfrAGO7.png" style="max-width: 100.0%;max-height: 100.0%;"> because edge <img align="middle" class="tex-formula" src="file://NaGupCWq.png" style="max-width: 100.0%;max-height: 100.0%;"> appears earlier in the input than the other two edges and hence cannot be picked/traversed after either of the other two edges.</p><p>In the second sample, it's optimal to pick <span class="tex-span">1</span>-st, <span class="tex-span">3</span>-rd and <span class="tex-span">5</span>-th edges to get the optimal answer: <img align="middle" class="tex-formula" src="file://iwVGPTSP.png" style="max-width: 100.0%;max-height: 100.0%;">. </p>
