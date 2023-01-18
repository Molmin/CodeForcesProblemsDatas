## Description

<div><p>You are given a weighted directed graph, consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. You should answer <span class="tex-span"><i>q</i></span> queries of two types:</p><ul> <li> <span class="tex-font-style-tt">1 v</span>&nbsp;— find the length of shortest path from vertex <span class="tex-span">1</span> to vertex <span class="tex-span"><i>v</i></span>. </li><li> <span class="tex-font-style-tt">2 c <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> <i>l</i><sub class="lower-index">2</sub> ... <i>l</i><sub class="lower-index"><i>c</i></sub></span></span>&nbsp;— add <span class="tex-span">1</span> to weights of edges with indices <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>c</i></sub></span>. </li></ul></div><div class="input-specification"><p>The first line of input data contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 2000</span>)&nbsp;— the number of vertices and edges in the graph, and the number of requests correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines of input data contain the descriptions of edges: <span class="tex-span"><i>i</i></span>-th of them contains description of edge with index <span class="tex-span"><i>i</i></span>&nbsp;— three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the beginning and the end of edge, and its initial weight correspondingly.</p><p>Next <span class="tex-span"><i>q</i></span> lines of input data contain the description of edges in the format described above (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>m</i></span>). It's guaranteed that inside single query all <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> are distinct. Also, it's guaranteed that a total number of edges in all requests of the second type does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>For each query of first type print the length of the shortest path from <span class="tex-span">1</span> to <span class="tex-span"><i>v</i></span> in a separate line. Print <span class="tex-font-style-tt">-1</span>, if such path does not exists.</p></div>

## Input

<p>The first line of input data contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 2000</span>)&nbsp;— the number of vertices and edges in the graph, and the number of requests correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines of input data contain the descriptions of edges: <span class="tex-span"><i>i</i></span>-th of them contains description of edge with index <span class="tex-span"><i>i</i></span>&nbsp;— three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the beginning and the end of edge, and its initial weight correspondingly.</p><p>Next <span class="tex-span"><i>q</i></span> lines of input data contain the description of edges in the format described above (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>m</i></span>). It's guaranteed that inside single query all <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> are distinct. Also, it's guaranteed that a total number of edges in all requests of the second type does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>For each query of first type print the length of the shortest path from <span class="tex-span">1</span> to <span class="tex-span"><i>v</i></span> in a separate line. Print <span class="tex-font-style-tt">-1</span>, if such path does not exists.</p>





```input1
3 2 9
1 2 0
2 3 0
2 1 2
1 3
1 2
2 1 1
1 3
1 2
2 2 1 2
1 3
1 2

```




```input2
5 4 9
2 3 1
2 4 1
3 4 1
1 2 0
1 5
1 4
2 1 2
2 1 2
1 4
2 2 1 3
1 4
2 1 4
1 4

```




```output1
1
0
2
1
4
2

```




```output2
-1
1
2
3
4

```



## Note

<center><p>The description of changes of the graph in the first sample case:</p><p><img class="tex-graphics" src="file://tsaoov3T.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The description of changes of the graph in the second sample case:</p><p><img class="tex-graphics" src="file://Lo0JzYyG.png" style="max-width: 100.0%;max-height: 100.0%;"></p></center>
