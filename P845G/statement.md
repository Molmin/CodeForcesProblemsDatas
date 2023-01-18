## Description

<div><p>You are given an undirected graph with weighted edges. The length of some path between two vertices is the bitwise xor of weights of all edges belonging to this path (if some edge is traversed more than once, then it is included in bitwise xor the same number of times). You have to find the minimum length of path between vertex <span class="tex-span">1</span> and vertex <span class="tex-span"><i>n</i></span>.</p><p><span class="tex-font-style-bf">Note that graph can contain multiple edges and loops. It is guaranteed that the graph is connected.</span></p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 100000</span>) — the number of vertices and the number of edges, respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each line containing three integer numbers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>w</i> ≤ 10<sup class="upper-index">8</sup></span>). These numbers denote an edge that connects vertices <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> and has weight <span class="tex-span"><i>w</i></span>.</p></div><div class="output-specification"><p>Print one number — the minimum length of path between vertices <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 100000</span>) — the number of vertices and the number of edges, respectively.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each line containing three integer numbers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>w</i> ≤ 10<sup class="upper-index">8</sup></span>). These numbers denote an edge that connects vertices <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> and has weight <span class="tex-span"><i>w</i></span>.</p>

## Output

<p>Print one number — the minimum length of path between vertices <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>.</p>





```input1
3 3
1 2 3
1 3 2
3 2 0

```




```input2
2 2
1 1 3
1 2 3

```




```output1
2

```




```output2
0

```


