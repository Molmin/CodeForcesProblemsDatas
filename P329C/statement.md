## Description

<div><p>I have an undirected graph consisting of <span class="tex-span"><i>n</i></span> nodes, numbered 1 through <span class="tex-span"><i>n</i></span>. Each node has at most two incident edges. For each pair of nodes, there is at most an edge connecting them. No edge connects a node to itself.</p><p>I would like to create a new graph in such a way that: </p><ul> <li> The new graph consists of the same number of nodes and edges as the old graph. </li><li> The properties in the first paragraph still hold. </li><li> For each two nodes <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>, if there is an edge connecting them in the old graph, there is no edge connecting them in the new graph. </li></ul><p>Help me construct the new graph, or tell me if it is impossible.</p></div><div class="input-specification"><p>The first line consists of two space-separated integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the number of nodes and edges, respectively. Then <span class="tex-span"><i>m</i></span> lines follow. Each of the <span class="tex-span"><i>m</i></span> lines consists of two space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i>;&nbsp;<i>u</i> ≠ <i>v</i></span>), denoting an edge between nodes <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p></div><div class="output-specification"><p>If it is not possible to construct a new graph with the mentioned properties, output a single line consisting of -1. Otherwise, output exactly <span class="tex-span"><i>m</i></span> lines. Each line should contain a description of edge in the same way as used in the input format.</p></div>

## Input

<p>The first line consists of two space-separated integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the number of nodes and edges, respectively. Then <span class="tex-span"><i>m</i></span> lines follow. Each of the <span class="tex-span"><i>m</i></span> lines consists of two space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i>;&nbsp;<i>u</i> ≠ <i>v</i></span>), denoting an edge between nodes <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p>

## Output

<p>If it is not possible to construct a new graph with the mentioned properties, output a single line consisting of -1. Otherwise, output exactly <span class="tex-span"><i>m</i></span> lines. Each line should contain a description of edge in the same way as used in the input format.</p>





```input1
8 7
1 2
2 3
4 5
5 6
6 8
8 7
7 4

```




```input2
3 2
1 2
2 3

```




```input3
5 4
1 2
2 3
3 4
4 1

```




```output1
1 4
4 6
1 6
2 7
7 5
8 5
2 8

```




```output2
-1

```




```output3
1 3
3 5
5 2
2 4

```



## Note

<p>The old graph of the first example:</p><p><img class="tex-graphics" src="file://iWgWzcZg.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>A possible new graph for the first example:</p><p><img class="tex-graphics" src="file://0wesGswS.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the second example, we cannot create any new graph.</p><p>The old graph of the third example:</p><p><img class="tex-graphics" src="file://RkRaAM5E.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>A possible new graph for the third example:</p><p><img class="tex-graphics" src="file://Mu7FpZul.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
