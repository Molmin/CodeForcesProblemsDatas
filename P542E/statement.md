## Description

<div><p>Vova and Marina love offering puzzles to each other. Today Marina offered Vova to cope with the following task.</p><p>Vova has a non-directed graph consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges without loops and multiple edges. Let's define the operation of <span class="tex-font-style-it">contraction</span> two vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> that are <span class="tex-font-style-bf">not connected by an edge</span>. As a result of this operation vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are deleted and instead of them a new vertex <span class="tex-span"><i>x</i></span> is added into the graph, and also edges are drawn from it to all vertices that were connected with <span class="tex-span"><i>a</i></span> or with <span class="tex-span"><i>b</i></span> (specifically, if the vertex was connected with both <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, then also exactly one edge is added from <span class="tex-span"><i>x</i></span> to it). Thus, as a result of <span class="tex-font-style-it">contraction</span> again a non-directed graph is formed, it contains no loops nor multiple edges, and it contains <span class="tex-span">(<i>n</i> - 1)</span> vertices.</p><p>Vova must perform the <span class="tex-font-style-it">contraction</span> an arbitrary number of times to transform the given graph into a <span class="tex-font-style-it">chain</span> of the maximum length. A <span class="tex-font-style-it">chain</span> of length <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i> ≥ 0</span>) is a connected graph whose vertices can be numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i> + 1</span> so that the edges of the graph connect all pairs of vertices <span class="tex-span">(<i>i</i>, <i>i</i> + 1)</span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>) and only them. Specifically, the graph that consists of one vertex is a chain of length <span class="tex-span">0</span>. The vertices that are formed as a result of the <span class="tex-font-style-it">contraction</span> are allowed to be used in the following operations of <span class="tex-font-style-it">contraction</span>.</p><center> <img class="tex-graphics" src="file://FAxbNiNI.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The picture illustrates the contraction of two vertices marked by red.</span> </center><p>Help Vova cope with his girlfriend's task. Find the maximum length of the chain that can be obtained from the resulting graph or else determine that it is impossible to obtain the chain.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100 000</span>) — the number of vertices and the number of edges in the original graph.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of edges in the format <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), which means that there is an edge between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that there is at most one edge between each pair of vertexes.</p></div><div class="output-specification"><p>If it is impossible to obtain a chain from the given graph, print <span class="tex-span"> - 1</span>. Otherwise, print the maximum possible number of edges in the resulting chain.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100 000</span>) — the number of vertices and the number of edges in the original graph.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of edges in the format <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), which means that there is an edge between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that there is at most one edge between each pair of vertexes.</p>

## Output

<p>If it is impossible to obtain a chain from the given graph, print <span class="tex-span"> - 1</span>. Otherwise, print the maximum possible number of edges in the resulting chain.</p>





```input1
5 4
1 2
2 3
3 4
3 5

```




```input2
4 6
1 2
2 3
1 3
3 4
2 4
1 4

```




```input3
4 2
1 3
2 4

```




```output1
3

```




```output2
-1

```




```output3
2

```



## Note

<p>In the first sample test you can contract vertices <span class="tex-span">4</span> and <span class="tex-span">5</span> and obtain a chain of length <span class="tex-span">3</span>.</p><p>In the second sample test it is initially impossible to contract any pair of vertexes, so it is impossible to achieve the desired result.</p><p>In the third sample test you can contract vertices <span class="tex-span">1</span> and <span class="tex-span">2</span> and obtain a chain of length <span class="tex-span">2</span>.</p>
