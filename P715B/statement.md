## Description

<div><p>ZS the Coder has drawn an undirected graph of <span class="tex-span"><i>n</i></span> vertices numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span> and <span class="tex-span"><i>m</i></span> edges between them. Each edge of the graph is weighted, each weight is a <span class="tex-font-style-bf">positive integer</span>.</p><p>The next day, ZS the Coder realized that some of the weights were erased! So he wants to reassign <span class="tex-font-style-bf">positive integer</span> weight to each of the edges which weights were erased, so that the length of the shortest path between vertices <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> in the resulting graph is exactly <span class="tex-span"><i>L</i></span>. Can you help him?</p></div><div class="input-specification"><p>The first line contains five integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>L</i>, <i>s</i>, <i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000,  1 ≤ <i>m</i> ≤ 10 000,  1 ≤ <i>L</i> ≤ 10<sup class="upper-index">9</sup>,  0 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i> - 1,  <i>s</i> ≠ <i>t</i></span>)&nbsp;— the number of vertices, number of edges, the desired length of shortest path, starting vertex and ending vertex respectively.</p><p>Then, <span class="tex-span"><i>m</i></span> lines describing the edges of the graph follow. <span class="tex-span"><i>i</i></span>-th of them contains three integers, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1,  <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>,  0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> denote the endpoints of the edge and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> denotes its weight. If <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is equal to <span class="tex-span">0</span> then the weight of the corresponding edge was erased.</p><p>It is guaranteed that there is at most one edge between any pair of vertices.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the only line if it's not possible to assign the weights in a required way.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line. Next <span class="tex-span"><i>m</i></span> lines should contain the edges of the resulting graph, with weights assigned to edges which weights were erased. <span class="tex-span"><i>i</i></span>-th of them should contain three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, denoting an edge between vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> of weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. The edges of the new graph must coincide with the ones in the graph from the input. The weights that were not erased must remain unchanged whereas the new weights can be any <span class="tex-font-style-bf">positive integer</span> not exceeding <span class="tex-span">10<sup class="upper-index">18</sup></span>. </p><p>The order of the edges in the output doesn't matter. The length of the shortest path between <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> must be equal to <span class="tex-span"><i>L</i></span>.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains five integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>L</i>, <i>s</i>, <i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000,  1 ≤ <i>m</i> ≤ 10 000,  1 ≤ <i>L</i> ≤ 10<sup class="upper-index">9</sup>,  0 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i> - 1,  <i>s</i> ≠ <i>t</i></span>)&nbsp;— the number of vertices, number of edges, the desired length of shortest path, starting vertex and ending vertex respectively.</p><p>Then, <span class="tex-span"><i>m</i></span> lines describing the edges of the graph follow. <span class="tex-span"><i>i</i></span>-th of them contains three integers, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1,  <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>,  0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> denote the endpoints of the edge and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> denotes its weight. If <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is equal to <span class="tex-span">0</span> then the weight of the corresponding edge was erased.</p><p>It is guaranteed that there is at most one edge between any pair of vertices.</p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the only line if it's not possible to assign the weights in a required way.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line. Next <span class="tex-span"><i>m</i></span> lines should contain the edges of the resulting graph, with weights assigned to edges which weights were erased. <span class="tex-span"><i>i</i></span>-th of them should contain three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, denoting an edge between vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> of weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. The edges of the new graph must coincide with the ones in the graph from the input. The weights that were not erased must remain unchanged whereas the new weights can be any <span class="tex-font-style-bf">positive integer</span> not exceeding <span class="tex-span">10<sup class="upper-index">18</sup></span>. </p><p>The order of the edges in the output doesn't matter. The length of the shortest path between <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> must be equal to <span class="tex-span"><i>L</i></span>.</p><p>If there are multiple solutions, print any of them.</p>





```input1
5 5 13 0 4
0 1 5
2 1 2
3 2 3
1 4 0
4 3 4

```




```input2
2 1 123456789 0 1
0 1 0

```




```input3
2 1 999999999 1 0
0 1 1000000000

```




```output1
YES
0 1 5
2 1 2
3 2 3
1 4 8
4 3 4

```




```output2
YES
0 1 123456789

```




```output3
NO

```



## Note

<p>Here's how the graph in the first sample case looks like :</p><center> <img class="tex-graphics" src="file://QIVctUM9.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the first sample case, there is only one missing edge weight. Placing the weight of <span class="tex-span">8</span> gives a shortest path from <span class="tex-span">0</span> to <span class="tex-span">4</span> of length <span class="tex-span">13</span>.</p><p>In the second sample case, there is only a single edge. Clearly, the only way is to replace the missing weight with <span class="tex-span">123456789</span>.</p><p>In the last sample case, there is no weights to assign but the length of the shortest path doesn't match the required value, so the answer is "<span class="tex-font-style-tt">NO</span>".</p>
