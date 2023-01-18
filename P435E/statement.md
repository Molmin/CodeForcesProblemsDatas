## Description

<div><p>In this problem you will need to deal with an <span class="tex-span"><i>n</i> × <i>m</i></span> grid graph. The graph's vertices are the nodes of the <span class="tex-span"><i>n</i> × <i>m</i></span> grid. The graph's edges are all the sides and diagonals of the grid's unit squares.</p><p>The figure below shows a <span class="tex-span">3 × 5</span> graph. The black lines are the graph's edges, the colored circles are the graph's vertices. The vertices of the graph are painted on the picture for a reason: the coloring is a correct vertex coloring of the <span class="tex-span">3 × 5</span> graph into four colors. A graph coloring is correct if and only if each vertex is painted and no two vertices connected by an edge are painted the same color.</p><center> <img class="tex-graphics" src="file://TGyxXyd4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given the size of the grid graph <span class="tex-span"><i>n</i> × <i>m</i></span> and the colors of some of its vertices. Find any way how to paint the unpainted vertices of the graph in 4 colors to make the final coloring a correct vertex graph coloring. If there is no such correct vertex coloring, say that the answer doesn't exist.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 1000)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines consists of <span class="tex-span"><i>m</i></span> characters — the given graph. Each character is either «<span class="tex-font-style-tt">0</span>», «<span class="tex-font-style-tt">1</span>», «<span class="tex-font-style-tt">2</span>», «<span class="tex-font-style-tt">3</span>», «<span class="tex-font-style-tt">4</span>». Character «<span class="tex-font-style-tt">0</span>» means that the corresponding vertex is unpainted, otherwise the character means the color of the vertex.</p><p>Assume that all the available colors are numbered from <span class="tex-span">1</span> to <span class="tex-span">4</span>.</p></div><div class="output-specification"><p>If there is no way to get correct vertex coloring of the graph, print 0 in a single line. Otherwise print the colored <span class="tex-span"><i>n</i> × <i>m</i></span> graph. Print the graph in the same format as in the input.</p><p>If multiple answers exist, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 1000)</span>. Each of the next <span class="tex-span"><i>n</i></span> lines consists of <span class="tex-span"><i>m</i></span> characters — the given graph. Each character is either «<span class="tex-font-style-tt">0</span>», «<span class="tex-font-style-tt">1</span>», «<span class="tex-font-style-tt">2</span>», «<span class="tex-font-style-tt">3</span>», «<span class="tex-font-style-tt">4</span>». Character «<span class="tex-font-style-tt">0</span>» means that the corresponding vertex is unpainted, otherwise the character means the color of the vertex.</p><p>Assume that all the available colors are numbered from <span class="tex-span">1</span> to <span class="tex-span">4</span>.</p>

## Output

<p>If there is no way to get correct vertex coloring of the graph, print 0 in a single line. Otherwise print the colored <span class="tex-span"><i>n</i> × <i>m</i></span> graph. Print the graph in the same format as in the input.</p><p>If multiple answers exist, print any of them.</p>





```input1
3 5
10101
00020
01000

```




```input2
2 2
00
00

```




```input3
2 2
11
00

```




```output1
13131
42424
31313

```




```output2
12
34

```




```output3
0

```



## Note

<p>The answer to the first sample is shown on the picture (1 — green color, 2 — blue, 3 — dark blue, 4 — pink).</p><p>In the second sample there exists 4! answers, each of them is considered correct.</p><p>In the third sample two vertices with equal colors are connected. So the correct vertex coloring couldn't be obtained.</p>
