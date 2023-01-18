## Description

<div><p>After Vitaly was expelled from the university, he became interested in the graph theory.</p><p>Vitaly especially liked the cycles of an odd length in which each vertex occurs at most once.</p><p>Vitaly was wondering how to solve the following problem. You are given an undirected graph consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges, not necessarily connected, without parallel edges and loops. You need to find <span class="tex-span"><i>t</i></span> — the minimum number of edges that must be added to the given graph in order to form a simple cycle of an odd length, consisting of more than one vertex. Moreover, he must find <span class="tex-span"><i>w</i></span> — the number of ways to add <span class="tex-span"><i>t</i></span> edges in order to form a cycle of an odd length (consisting of more than one vertex). It is prohibited to add loops or parallel edges.</p><p>Two ways to add edges to the graph are considered equal if they have the same sets of added edges.</p><p>Since Vitaly does not study at the university, he asked you to help him with this task.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://9Q621WEE.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;—&nbsp;the number of vertices in the graph and the number of edges in the graph.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the edges of the graph, one edge per line. Each edge is given by a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;—&nbsp;the vertices that are connected by the <span class="tex-span"><i>i</i></span>-th edge. All numbers in the lines are separated by a single space.</p><p>It is guaranteed that the given graph doesn't contain any loops and parallel edges. The graph isn't necessarily connected.</p></div><div class="output-specification"><p>Print in the first line of the output two space-separated integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>w</i></span>&nbsp;—&nbsp;the minimum number of edges that should be added to the graph to form a simple cycle of an odd length consisting of more than one vertex where each vertex occurs at most once, and the number of ways to do this.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://9Q621WEE.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;—&nbsp;the number of vertices in the graph and the number of edges in the graph.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the edges of the graph, one edge per line. Each edge is given by a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;—&nbsp;the vertices that are connected by the <span class="tex-span"><i>i</i></span>-th edge. All numbers in the lines are separated by a single space.</p><p>It is guaranteed that the given graph doesn't contain any loops and parallel edges. The graph isn't necessarily connected.</p>

## Output

<p>Print in the first line of the output two space-separated integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>w</i></span>&nbsp;—&nbsp;the minimum number of edges that should be added to the graph to form a simple cycle of an odd length consisting of more than one vertex where each vertex occurs at most once, and the number of ways to do this.</p>





```input1
4 4
1 2
1 3
4 2
4 3

```




```input2
3 3
1 2
2 3
3 1

```




```input3
3 0

```




```output1
1 2

```




```output2
0 1

```




```output3
3 1

```



## Note

<p>The simple cycle is a cycle that doesn't contain any vertex twice.</p>
