## Description

<div><p>Little Chris is participating in a graph cutting contest. He's a pro. The time has come to test his skills to the fullest.</p><p>Chris is given a simple undirected connected graph with <span class="tex-span"><i>n</i></span> vertices (numbered from 1 to <span class="tex-span"><i>n</i></span>) and <span class="tex-span"><i>m</i></span> edges. The problem is to cut it into edge-distinct paths of length 2. Formally, Chris has to partition all edges of the graph into pairs in such a way that the edges in a single pair are adjacent and each edge must be contained in exactly one pair.</p><p>For example, the figure shows a way Chris can cut a graph. The first sample test contains the description of this graph.</p><center> <img class="tex-graphics" src="file://LldN5fOQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given a chance to compete with Chris. Find a way to cut the given graph or determine that it is impossible!</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of vertices and the number of edges in the graph. The next <span class="tex-span"><i>m</i></span> lines contain the description of the graph's edges. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), the numbers of the vertices connected by the <span class="tex-span"><i>i</i></span>-th edge. It is guaranteed that the given graph is simple (without self-loops and multi-edges) and connected.</p><p><span class="tex-font-style-bf">Note</span>: since the size of the input and output could be very large, don't use slow output techniques in your language. For example, do not use input and output streams (cin, cout) in C++.</p></div><div class="output-specification"><p>If it is possible to cut the given graph into edge-distinct paths of length 2, output <img align="middle" class="tex-formula" src="file://ilkoPYS5.png" style="max-width: 100.0%;max-height: 100.0%;"> lines. In the <span class="tex-span"><i>i</i></span>-th line print three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span>, the description of the <span class="tex-span"><i>i</i></span>-th path. The graph should contain this path, i.e., the graph should contain edges <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> and <span class="tex-span">(<i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub>)</span>. Each edge should appear in exactly one path of length 2. If there are multiple solutions, output any of them.</p><p>If it is impossible to cut the given graph, print <span class="tex-font-style-tt">"No solution"</span> (without quotes).</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of vertices and the number of edges in the graph. The next <span class="tex-span"><i>m</i></span> lines contain the description of the graph's edges. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), the numbers of the vertices connected by the <span class="tex-span"><i>i</i></span>-th edge. It is guaranteed that the given graph is simple (without self-loops and multi-edges) and connected.</p><p><span class="tex-font-style-bf">Note</span>: since the size of the input and output could be very large, don't use slow output techniques in your language. For example, do not use input and output streams (cin, cout) in C++.</p>

## Output

<p>If it is possible to cut the given graph into edge-distinct paths of length 2, output <img align="middle" class="tex-formula" src="file://ilkoPYS5.png" style="max-width: 100.0%;max-height: 100.0%;"> lines. In the <span class="tex-span"><i>i</i></span>-th line print three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span>, the description of the <span class="tex-span"><i>i</i></span>-th path. The graph should contain this path, i.e., the graph should contain edges <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> and <span class="tex-span">(<i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub>)</span>. Each edge should appear in exactly one path of length 2. If there are multiple solutions, output any of them.</p><p>If it is impossible to cut the given graph, print <span class="tex-font-style-tt">"No solution"</span> (without quotes).</p>





```input1
8 12
1 2
2 3
3 4
4 1
1 3
2 4
3 5
3 6
5 6
6 7
6 8
7 8

```




```input2
3 3
1 2
2 3
3 1

```




```input3
3 2
1 2
2 3

```




```output1
1 2 4
1 3 2
1 4 3
5 3 6
5 6 8
6 7 8
```




```output2
No solution

```




```output3
1 2 3

```


