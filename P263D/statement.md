## Description

<div><p>You've got a undirected graph <span class="tex-span"><i>G</i></span>, consisting of <span class="tex-span"><i>n</i></span> nodes. We will consider the nodes of the graph indexed by integers from 1 to <span class="tex-span"><i>n</i></span>. We know that each node of graph <span class="tex-span"><i>G</i></span> is connected by edges with at least <span class="tex-span"><i>k</i></span> other nodes of this graph. Your task is to find in the given graph a simple cycle of length of at least <span class="tex-span"><i>k</i> + 1</span>.</p><p>A <span class="tex-font-style-it">simple cycle</span> of length <span class="tex-span"><i>d</i></span> <span class="tex-span">(<i>d</i> &gt; 1)</span> in graph <span class="tex-span"><i>G</i></span> is a sequence of distinct graph nodes <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>d</i></sub></span> such, that nodes <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>d</i></sub></span> are connected by an edge of the graph, also for any integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>d</i>)</span> nodes <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> are connected by an edge of the graph.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(3 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;2 ≤ <i>k</i> ≤ <i>n</i> - 1)</span> — the number of the nodes of the graph, the number of the graph's edges and the lower limit on the degree of the graph node. Next <span class="tex-span"><i>m</i></span> lines contain pairs of integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the indexes of the graph nodes that are connected by the <span class="tex-span"><i>i</i></span>-th edge. </p><p>It is guaranteed that the given graph doesn't contain any multiple edges or self-loops. It is guaranteed that each node of the graph is connected by the edges with at least <span class="tex-span"><i>k</i></span> other nodes of the graph.</p></div><div class="output-specification"><p>In the first line print integer <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>r</i> ≥ <i>k</i> + 1)</span> — the length of the found cycle. In the next line print <span class="tex-span"><i>r</i></span> distinct integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>r</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the found simple cycle.</p><p>It is guaranteed that the answer exists. If there are multiple correct answers, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(3 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;2 ≤ <i>k</i> ≤ <i>n</i> - 1)</span> — the number of the nodes of the graph, the number of the graph's edges and the lower limit on the degree of the graph node. Next <span class="tex-span"><i>m</i></span> lines contain pairs of integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the indexes of the graph nodes that are connected by the <span class="tex-span"><i>i</i></span>-th edge. </p><p>It is guaranteed that the given graph doesn't contain any multiple edges or self-loops. It is guaranteed that each node of the graph is connected by the edges with at least <span class="tex-span"><i>k</i></span> other nodes of the graph.</p>

## Output

<p>In the first line print integer <span class="tex-span"><i>r</i></span> <span class="tex-span">(<i>r</i> ≥ <i>k</i> + 1)</span> — the length of the found cycle. In the next line print <span class="tex-span"><i>r</i></span> distinct integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>r</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the found simple cycle.</p><p>It is guaranteed that the answer exists. If there are multiple correct answers, you are allowed to print any of them.</p>





```input1
3 3 2
1 2
2 3
3 1

```




```input2
4 6 3
4 3
1 2
1 3
1 4
2 3
2 4

```




```output1
3
1 2 3
```




```output2
4
3 4 1 2
```


