## Description

<div><p>Given a simple graph, output the number of simple cycles in it. A simple cycle is a cycle with no repeated vertices or edges.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 19</span>, <span class="tex-span">0 ≤ <i>m</i></span>) – respectively the number of vertices and edges of the graph. Each of the subsequent <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>) indicating that vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are connected by an undirected edge. There is no more than one edge connecting any pair of vertices.</p></div><div class="output-specification"><p>Output the number of cycles in the given graph.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 19</span>, <span class="tex-span">0 ≤ <i>m</i></span>) – respectively the number of vertices and edges of the graph. Each of the subsequent <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>) indicating that vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are connected by an undirected edge. There is no more than one edge connecting any pair of vertices.</p>

## Output

<p>Output the number of cycles in the given graph.</p>





```input1
4 6
1 2
1 3
1 4
2 3
2 4
3 4

```




```output1
7

```



## Note

<p>The example graph is a clique and contains four cycles of length 3 and three cycles of length 4.</p>
