## Description

<div><p>You are given a weighted undirected graph. The vertices are enumerated from 1 to <span class="tex-span"><i>n</i></span>. Your task is to find the shortest path between the vertex <span class="tex-span">1</span> and the vertex <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> is the number of vertices and <span class="tex-span"><i>m</i></span> is the number of edges. Following <span class="tex-span"><i>m</i></span> lines contain one edge each in form <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> are edge endpoints and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is the length of the edge.</p><p>It is possible that the graph has loops and multiple edges between pair of vertices.</p></div><div class="output-specification"><p>Write the only integer <span class="tex-font-style-tt">-1</span> in case of no path. Write the shortest path in opposite case. If there are many solutions, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> is the number of vertices and <span class="tex-span"><i>m</i></span> is the number of edges. Following <span class="tex-span"><i>m</i></span> lines contain one edge each in form <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> are edge endpoints and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is the length of the edge.</p><p>It is possible that the graph has loops and multiple edges between pair of vertices.</p>

## Output

<p>Write the only integer <span class="tex-font-style-tt">-1</span> in case of no path. Write the shortest path in opposite case. If there are many solutions, print any of them.</p>





```input1
5 6
1 2 2
2 5 5
2 3 4
1 4 1
4 3 3
3 5 1

```




```input2
5 6
1 2 2
2 5 5
2 3 4
1 4 1
4 3 3
3 5 1

```




```output1
1 4 3 5
```




```output2
1 4 3 5
```


