## Description

<div><p>Jamie has recently found undirected weighted graphs with the following properties very <span class="tex-font-style-tt">interesting</span>:</p><ul> <li> The graph is connected and contains exactly <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. </li><li> All edge weights are integers and are in range <span class="tex-span">[1, 10<sup class="upper-index">9</sup>]</span> inclusive. </li><li> The length of shortest path from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> is a prime number. </li><li> The sum of edges' weights in the minimum spanning tree (MST) of the graph is a prime number. </li><li> The graph contains no loops or multi-edges. </li></ul><p>If you are not familiar with some terms from the statement you can find definitions of them in notes section. </p><p>Help Jamie construct any graph with given number of vertices and edges that is <span class="tex-font-style-tt">interesting</span>!</p></div><div class="input-specification"><p>First line of input contains 2 integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://IFGO1dPC.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— the required number of vertices and edges.</p></div><div class="output-specification"><p>In the first line output 2 integers <span class="tex-span"><i>sp</i></span>, <span class="tex-span"><i>mstw</i></span> <span class="tex-span">(1 ≤ <i>sp</i>, <i>mstw</i> ≤ 10<sup class="upper-index">14</sup>)</span>&nbsp;— the length of the shortest path and the sum of edges' weights in the minimum spanning tree.</p><p>In the next <span class="tex-span"><i>m</i></span> lines output the edges of the graph. In each line output 3 integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>w</i></span> <span class="tex-span">(1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i>, 1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup>)</span> describing the edge connecting <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> and having weight <span class="tex-span"><i>w</i></span>. </p></div>

## Input

<p>First line of input contains 2 integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://IFGO1dPC.png" style="max-width: 100.0%;max-height: 100.0%;">&nbsp;— the required number of vertices and edges.</p>

## Output

<p>In the first line output 2 integers <span class="tex-span"><i>sp</i></span>, <span class="tex-span"><i>mstw</i></span> <span class="tex-span">(1 ≤ <i>sp</i>, <i>mstw</i> ≤ 10<sup class="upper-index">14</sup>)</span>&nbsp;— the length of the shortest path and the sum of edges' weights in the minimum spanning tree.</p><p>In the next <span class="tex-span"><i>m</i></span> lines output the edges of the graph. In each line output 3 integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>w</i></span> <span class="tex-span">(1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i>, 1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup>)</span> describing the edge connecting <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> and having weight <span class="tex-span"><i>w</i></span>. </p>





```input1
4 4

```




```input2
5 4

```




```output1
7 7
1 2 3
2 3 2
3 4 2
2 4 4

```




```output2
7 13
1 2 2
1 3 4
1 4 3
4 5 4

```



## Note

<p><span class="tex-font-style-bf">The graph of sample 1:</span> <img class="tex-graphics" src="file://H2VeNrGx.png" style="max-width: 100.0%;max-height: 100.0%;"> Shortest path sequence: <span class="tex-span">{1, 2, 3, 4}</span>. MST edges are marked with an asterisk (*).</p><p><span class="tex-font-style-bf">Definition of terms used in the problem statement:</span></p><p>A <span class="tex-font-style-bf">shortest path</span> in an undirected graph is a sequence of vertices <span class="tex-span">(<i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ... , <i>v</i><sub class="lower-index"><i>k</i></sub>)</span> such that <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> is adjacent to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> <span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span> and the sum of weight <img align="middle" class="tex-formula" src="file://PgidaTN2.png" style="max-width: 100.0%;max-height: 100.0%;"> is minimized where <span class="tex-span"><i>w</i>(<i>i</i>, <i>j</i>)</span> is the edge weight between <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. (<a href="https://en.wikipedia.org/wiki/Shortest_path_problem">https://en.wikipedia.org/wiki/Shortest_path_problem</a>)</p><p>A <span class="tex-font-style-bf">prime number</span> is a natural number greater than 1 that has no positive divisors other than 1 and itself. (<a href="https://en.wikipedia.org/wiki/Prime_number">https://en.wikipedia.org/wiki/Prime_number</a>)</p><p>A <span class="tex-font-style-bf">minimum spanning tree (MST)</span> is a subset of the edges of a connected, edge-weighted undirected graph that connects all the vertices together, without any cycles and with the minimum possible total edge weight. (<a href="https://en.wikipedia.org/wiki/Minimum_spanning_tree">https://en.wikipedia.org/wiki/Minimum_spanning_tree</a>)</p><p><a href="https://en.wikipedia.org/wiki/Multiple_edges">https://en.wikipedia.org/wiki/Multiple_edges</a></p>
