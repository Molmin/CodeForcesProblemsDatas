## Description

<div><p>You are given a complete undirected graph with <span class="tex-span"><i>n</i></span> vertices. A number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is assigned to each vertex, and the weight of an edge between vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> <i>xor</i> <i>a</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>Calculate the weight of the minimum spanning tree in this graph.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the number of vertices in the graph.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) — the numbers assigned to the vertices.</p></div><div class="output-specification"><p>Print one number — the weight of the minimum spanning tree in the graph.</p></div>

## Input

<p>The first line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the number of vertices in the graph.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) — the numbers assigned to the vertices.</p>

## Output

<p>Print one number — the weight of the minimum spanning tree in the graph.</p>





```input1
5
1 2 3 4 5

```




```input2
4
1 2 3 4

```




```output1
8

```




```output2
8

```


