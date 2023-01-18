## Description

<div><p>Fox Ciel wants to write a task for a programming contest. The task is: "You are given a simple undirected graph with <span class="tex-span"><i>n</i></span> vertexes. Each its edge has unit length. You should calculate the number of shortest paths between vertex 1 and vertex 2."</p><p>Same with some writers, she wants to make an example with some certain output: for example, her birthday or the number of her boyfriend. Can you help her to make a test case with answer equal exactly to <span class="tex-span"><i>k</i></span>?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>You should output a graph <span class="tex-span"><i>G</i></span> with <span class="tex-span"><i>n</i></span> vertexes (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>). There must be exactly <span class="tex-span"><i>k</i></span> shortest paths between vertex 1 and vertex 2 of the graph.</p><p>The first line must contain an integer <span class="tex-span"><i>n</i></span>. Then adjacency matrix <span class="tex-span"><i>G</i></span> with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns must follow. Each element of the matrix must be '<span class="tex-font-style-tt">N</span>' or '<span class="tex-font-style-tt">Y</span>'. If <span class="tex-span"><i>G</i><sub class="lower-index"><i>ij</i></sub></span> is '<span class="tex-font-style-tt">Y</span>', then graph <span class="tex-span"><i>G</i></span> has a edge connecting vertex <span class="tex-span"><i>i</i></span> and vertex <span class="tex-span"><i>j</i></span>. Consider the graph vertexes are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p><p>The graph must be undirected and simple: <span class="tex-span"><i>G</i><sub class="lower-index"><i>ii</i></sub></span> = '<span class="tex-font-style-tt">N</span>' and <span class="tex-span"><i>G</i><sub class="lower-index"><i>ij</i></sub> = <i>G</i><sub class="lower-index"><i>ji</i></sub></span> must hold. And there must be at least one path between vertex 1 and vertex 2. It's guaranteed that the answer exists. If there multiple correct answers, you can output any of them. </p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>You should output a graph <span class="tex-span"><i>G</i></span> with <span class="tex-span"><i>n</i></span> vertexes (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>). There must be exactly <span class="tex-span"><i>k</i></span> shortest paths between vertex 1 and vertex 2 of the graph.</p><p>The first line must contain an integer <span class="tex-span"><i>n</i></span>. Then adjacency matrix <span class="tex-span"><i>G</i></span> with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns must follow. Each element of the matrix must be '<span class="tex-font-style-tt">N</span>' or '<span class="tex-font-style-tt">Y</span>'. If <span class="tex-span"><i>G</i><sub class="lower-index"><i>ij</i></sub></span> is '<span class="tex-font-style-tt">Y</span>', then graph <span class="tex-span"><i>G</i></span> has a edge connecting vertex <span class="tex-span"><i>i</i></span> and vertex <span class="tex-span"><i>j</i></span>. Consider the graph vertexes are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p><p>The graph must be undirected and simple: <span class="tex-span"><i>G</i><sub class="lower-index"><i>ii</i></sub></span> = '<span class="tex-font-style-tt">N</span>' and <span class="tex-span"><i>G</i><sub class="lower-index"><i>ij</i></sub> = <i>G</i><sub class="lower-index"><i>ji</i></sub></span> must hold. And there must be at least one path between vertex 1 and vertex 2. It's guaranteed that the answer exists. If there multiple correct answers, you can output any of them. </p>





```input1
2
```




```input2
9
```




```input3
1
```




```output1
4
NNYY
NNYY
YYNN
YYNN
```




```output2
8
NNYYYNNN
NNNNNYYY
YNNNNYYY
YNNNNYYY
YNNNNYYY
NYYYYNNN
NYYYYNNN
NYYYYNNN
```




```output3
2
NY
YN
```



## Note

<p>In first example, there are 2 shortest paths: 1-3-2 and 1-4-2.</p><p>In second example, there are 9 shortest paths: 1-3-6-2, 1-3-7-2, 1-3-8-2, 1-4-6-2, 1-4-7-2, 1-4-8-2, 1-5-6-2, 1-5-7-2, 1-5-8-2.</p>
