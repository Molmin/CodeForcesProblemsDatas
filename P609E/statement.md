## Description

<div><p>Connected undirected weighted graph without self-loops and multiple edges is given. Graph contains <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges.</p><p>For each edge <span class="tex-span">(<i>u</i>, <i>v</i>)</span> find the minimal possible weight of the spanning tree that contains the edge <span class="tex-span">(<i>u</i>, <i>v</i>)</span>.</p><p>The weight of the spanning tree is the sum of weights of all edges included in spanning tree.</p></div><div class="input-specification"><p>First line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, <i>n</i> - 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of vertices and edges in graph.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the endpoints of the <span class="tex-span"><i>i</i></span>-th edge and its weight.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines. <span class="tex-span"><i>i</i></span>-th line should contain the minimal possible weight of the spanning tree that contains <span class="tex-span"><i>i</i></span>-th edge.</p><p>The edges are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in order of their appearing in input.</p></div>

## Input

<p>First line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, <i>n</i> - 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of vertices and edges in graph.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the endpoints of the <span class="tex-span"><i>i</i></span>-th edge and its weight.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines. <span class="tex-span"><i>i</i></span>-th line should contain the minimal possible weight of the spanning tree that contains <span class="tex-span"><i>i</i></span>-th edge.</p><p>The edges are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in order of their appearing in input.</p>





```input1
5 7
1 2 3
1 3 1
1 4 5
2 3 2
2 5 3
3 4 2
4 5 4

```




```output1
9
8
11
8
8
8
9

```


