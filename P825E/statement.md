## Description

<div><p>You are given a directed acyclic graph with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. There are no self-loops or multiple edges between any pair of vertices. Graph can be disconnected.</p><p>You should assign labels to all vertices in such a way that:</p><ul> <li> Labels form a valid permutation of length <span class="tex-span"><i>n</i></span> — an integer sequence such that each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> appears exactly once in it. </li><li> If there exists an edge from vertex <span class="tex-span"><i>v</i></span> to vertex <span class="tex-span"><i>u</i></span> then <span class="tex-span"><i>label</i><sub class="lower-index"><i>v</i></sub></span> should be smaller than <span class="tex-span"><i>label</i><sub class="lower-index"><i>u</i></sub></span>. </li><li> Permutation should be lexicographically smallest among all suitable. </li></ul><p>Find such sequence of labels to satisfy all the conditions.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain two integer numbers <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i>, <i>v</i> ≠ <i>u</i></span>) — edges of the graph. Edges are directed, graph doesn't contain loops or multiple edges.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> numbers — lexicographically smallest correct permutation of labels of vertices.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain two integer numbers <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i>, <i>v</i> ≠ <i>u</i></span>) — edges of the graph. Edges are directed, graph doesn't contain loops or multiple edges.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> numbers — lexicographically smallest correct permutation of labels of vertices.</p>





```input1
3 3
1 2
1 3
3 2

```




```input2
4 5
3 1
4 1
2 3
3 4
2 4

```




```input3
5 4
3 1
2 1
2 3
4 5

```




```output1
1 3 2 

```




```output2
4 1 2 3 

```




```output3
3 1 2 4 5 

```


