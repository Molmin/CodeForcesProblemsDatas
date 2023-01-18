## Description

<div><p>You are given an undirected graph consisting of <span class="tex-span"><i>n</i></span> vertices. Initially there are no edges in the graph. Also you are given <span class="tex-span"><i>q</i></span> queries, each query either adds one undirected edge to the graph or removes it. After each query you have to check if the resulting graph is bipartite (that is, you can paint all vertices of the graph into two colors so that there is no edge connecting two vertices of the same color).</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>q</i> ≤ 100000</span>).</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. <span class="tex-span"><i>i</i></span>th line contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). These numbers describe <span class="tex-span"><i>i</i></span>th query: if there is an edge between vertices <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, then remove it, otherwise add it.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines. <span class="tex-span"><i>i</i></span>th line must contain <span class="tex-font-style-tt">YES</span> if the graph is bipartite after <span class="tex-span"><i>i</i></span>th query, and <span class="tex-font-style-tt">NO</span> otherwise.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>q</i> ≤ 100000</span>).</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. <span class="tex-span"><i>i</i></span>th line contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). These numbers describe <span class="tex-span"><i>i</i></span>th query: if there is an edge between vertices <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, then remove it, otherwise add it.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines. <span class="tex-span"><i>i</i></span>th line must contain <span class="tex-font-style-tt">YES</span> if the graph is bipartite after <span class="tex-span"><i>i</i></span>th query, and <span class="tex-font-style-tt">NO</span> otherwise.</p>





```input1
3 5
2 3
1 3
1 2
1 2
1 2

```




```output1
YES
YES
NO
YES
NO

```


