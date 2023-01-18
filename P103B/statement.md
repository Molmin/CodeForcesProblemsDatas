## Description

<div><p>...Once upon a time a man came to the sea. The sea was stormy and dark. The man started to call for the little mermaid to appear but alas, he only woke up Cthulhu...</p><p>Whereas on the other end of the world Pentagon is actively collecting information trying to predict the monster's behavior and preparing the secret super weapon. Due to high seismic activity and poor weather conditions the satellites haven't yet been able to make clear shots of the monster. The analysis of the first shot resulted in an undirected graph with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. Now the world's best minds are about to determine whether this graph can be regarded as Cthulhu or not.</p><p>To add simplicity, let's suppose that Cthulhu looks from the space like some spherical body with tentacles attached to it. Formally, we shall regard as Cthulhu such an undirected graph that can be represented as a set of three or more rooted trees, whose roots are connected by a simple cycle.</p><p>It is guaranteed that the graph contains no multiple edges and self-loops.</p><center> <img class="tex-graphics" src="file://SsAP6UgA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The first line contains two integers — the number of vertices <span class="tex-span"><i>n</i></span> and the number of edges <span class="tex-span"><i>m</i></span> of the graph (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ </span><img align="middle" class="tex-formula" src="file://JjEj5VUn.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains a pair of integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, that show that an edge exists between vertices <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i></span>). For each pair of vertices there will be at most one edge between them, no edge connects a vertex to itself.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>", if the graph is not Cthulhu and "<span class="tex-font-style-tt">FHTAGN!</span>" if it is.</p></div>

## Input

<p>The first line contains two integers — the number of vertices <span class="tex-span"><i>n</i></span> and the number of edges <span class="tex-span"><i>m</i></span> of the graph (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ </span><img align="middle" class="tex-formula" src="file://JjEj5VUn.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains a pair of integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, that show that an edge exists between vertices <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i></span>). For each pair of vertices there will be at most one edge between them, no edge connects a vertex to itself.</p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>", if the graph is not Cthulhu and "<span class="tex-font-style-tt">FHTAGN!</span>" if it is.</p>





```input1
6 6
6 3
6 4
5 1
2 5
1 4
5 4

```




```input2
6 5
5 6
4 6
3 1
5 1
1 2

```




```output1
FHTAGN!
```




```output2
NO
```



## Note

<p>Let us denote as a simple cycle a set of <span class="tex-span"><i>v</i></span> vertices that can be numbered so that the edges will only exist between vertices number <span class="tex-span">1</span> and <span class="tex-span">2</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span>, ..., <span class="tex-span"><i>v</i> - 1</span> and <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span">1</span>.</p><p>A tree is a connected undirected graph consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>n</i> - 1</span> edges (<span class="tex-span"><i>n</i> &gt; 0</span>).</p><p>A rooted tree is a tree where one vertex is selected to be the root.</p>
