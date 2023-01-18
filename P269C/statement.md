## Description

<div><p>Emuskald considers himself a master of flow algorithms. Now he has completed his most ingenious program yet — it calculates the maximum flow in an undirected graph. The graph consists of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. Vertices are numbered from 1 to <span class="tex-span"><i>n</i></span>. Vertices <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> being the source and the sink respectively.</p><p>However, his max-flow algorithm seems to have a little flaw — it only finds the flow volume for each edge, but not its direction. Help him find for each edge the direction of the flow through this edges. Note, that the resulting flow should be correct maximum flow.</p><p>More formally. You are given an undirected graph. For each it's undirected edge (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>) you are given the flow volume <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. You should direct all edges in such way that the following conditions hold:</p><ol> <li> for each vertex <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 &lt; <i>v</i> &lt; <i>n</i>)</span>, sum of <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> of incoming edges is equal to the sum of <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> of outcoming edges; </li><li> vertex with number <span class="tex-span">1</span> has no incoming edges; </li><li> the obtained directed graph <span class="tex-font-style-bf">does not have cycles</span>. </li></ol></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>), the number of vertices and edges in the graph. The following <span class="tex-span"><i>m</i></span> lines contain three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), which means that there is an undirected edge from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with flow volume <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that there are no two edges connecting the same vertices; the given graph is connected; a solution always exists.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>m</i></span> lines, each containing one integer <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, which should be 0 if the direction of the <span class="tex-span"><i>i</i></span>-th edge is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> → <i>b</i><sub class="lower-index"><i>i</i></sub></span> (the flow goes from vertex <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to vertex <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>) and should be 1 otherwise. The edges are numbered from 1 to <span class="tex-span"><i>m</i></span> in the order they are given in the input.</p><p>If there are several solutions you can print any of them.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>), the number of vertices and edges in the graph. The following <span class="tex-span"><i>m</i></span> lines contain three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), which means that there is an undirected edge from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with flow volume <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that there are no two edges connecting the same vertices; the given graph is connected; a solution always exists.</p>

## Output

<p>Output <span class="tex-span"><i>m</i></span> lines, each containing one integer <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, which should be 0 if the direction of the <span class="tex-span"><i>i</i></span>-th edge is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> → <i>b</i><sub class="lower-index"><i>i</i></sub></span> (the flow goes from vertex <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to vertex <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>) and should be 1 otherwise. The edges are numbered from 1 to <span class="tex-span"><i>m</i></span> in the order they are given in the input.</p><p>If there are several solutions you can print any of them.</p>





```input1
3 3
3 2 10
1 2 10
3 1 5

```




```input2
4 5
1 2 10
1 3 10
2 3 5
4 2 15
3 4 5

```




```output1
1
0
1

```




```output2
0
0
1
1
0

```



## Note

<p>In the first test case, 10 flow units pass through path <img align="middle" class="tex-formula" src="file://PLS1khZ6.png" style="max-width: 100.0%;max-height: 100.0%;">, and 5 flow units pass directly from source to sink: <img align="middle" class="tex-formula" src="file://zfs4Vxrn.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
