## Description

<div><p><span class="tex-font-style-it">DZY loves Physics, and he enjoys calculating density.</span></p><p>Almost everything has density, even a graph. We define the density of a non-directed graph (nodes and edges of the graph have some values) as follows: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://hn97TRCl.png" style="max-width: 100.0%;max-height: 100.0%;"></center> where <span class="tex-span"><i>v</i></span> is the sum of the values of the nodes, <span class="tex-span"><i>e</i></span> is the sum of the values of the edges.<p>Once DZY got a graph <span class="tex-span"><i>G</i></span>, now he wants to find a connected induced subgraph <span class="tex-span"><i>G</i>'</span> of the graph, such that the density of <span class="tex-span"><i>G</i>'</span> is as large as possible.</p><p>An induced subgraph <span class="tex-span"><i>G</i>'(<i>V</i>', <i>E</i>')</span> of a graph <span class="tex-span"><i>G</i>(<i>V</i>, <i>E</i>)</span> is a graph that satisfies:</p><ul> <li> <img align="middle" class="tex-formula" src="file://m5EJwl6Y.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> edge <img align="middle" class="tex-formula" src="file://C6fL2WGw.png" style="max-width: 100.0%;max-height: 100.0%;"> if and only if <img align="middle" class="tex-formula" src="file://PpI8lIHL.png" style="max-width: 100.0%;max-height: 100.0%;">, and edge <img align="middle" class="tex-formula" src="file://VKdKlstl.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> the value of an edge in <span class="tex-span"><i>G</i>'</span> is the same as the value of the corresponding edge in <span class="tex-span"><i>G</i></span>, so as the value of a node. </li></ul><p>Help DZY to find the induced subgraph with maximum density. Note that the induced subgraph you choose must be connected.</p><center> <img class="tex-graphics" src="file://OwbKkd3S.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 500)</span>, <img align="middle" class="tex-formula" src="file://yATYYIGU.png" style="max-width: 100.0%;max-height: 100.0%;">. Integer <span class="tex-span"><i>n</i></span> represents the number of nodes of the graph <span class="tex-span"><i>G</i></span>, <span class="tex-span"><i>m</i></span> represents the number of edges.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> represents the value of the <span class="tex-span"><i>i</i></span>-th node. Consider the graph nodes are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup>)</span>, denoting an edge between node <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with value <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. The graph won't contain multiple edges.</p></div><div class="output-specification"><p>Output a real number denoting the answer, with an absolute or relative error of at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 500)</span>, <img align="middle" class="tex-formula" src="file://yATYYIGU.png" style="max-width: 100.0%;max-height: 100.0%;">. Integer <span class="tex-span"><i>n</i></span> represents the number of nodes of the graph <span class="tex-span"><i>G</i></span>, <span class="tex-span"><i>m</i></span> represents the number of edges.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> represents the value of the <span class="tex-span"><i>i</i></span>-th node. Consider the graph nodes are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup>)</span>, denoting an edge between node <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with value <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. The graph won't contain multiple edges.</p>

## Output

<p>Output a real number denoting the answer, with an absolute or relative error of at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
1 0
1

```




```input2
2 1
1 2
1 2 1

```




```input3
5 6
13 56 73 98 17
1 2 56
1 3 29
1 4 42
2 3 95
2 4 88
3 4 63

```




```output1
0.000000000000000

```




```output2
3.000000000000000

```




```output3
2.965517241379311

```



## Note

<p>In the first sample, you can only choose an empty subgraph, or the subgraph containing only node <span class="tex-span">1</span>.</p><p>In the second sample, choosing the whole graph is optimal.</p>
