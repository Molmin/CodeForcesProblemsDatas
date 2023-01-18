## Description

<div><p>Mahmoud and Ehab continue their adventures! As everybody in the evil land knows, Dr. Evil likes bipartite graphs, especially trees.</p><p>A tree is a connected acyclic graph. A bipartite graph is a graph, whose vertices can be partitioned into <span class="tex-span">2</span> sets in such a way, that for each edge <span class="tex-span">(<i>u</i>, <i>v</i>)</span> that belongs to the graph, <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> belong to different sets. You can find more formal definitions of a tree and a bipartite graph in the notes section below.</p><p>Dr. Evil gave Mahmoud and Ehab a tree consisting of <span class="tex-span"><i>n</i></span> nodes and asked them to add edges to it in such a way, that the graph is still bipartite. Besides, after adding these edges the graph should be simple (doesn't contain loops or multiple edges). What is the maximum number of edges they can add?</p><p>A loop is an edge, which connects a node with itself. Graph doesn't contain multiple edges when for each pair of nodes there is no more than one edge between them. <span class="tex-font-style-bf">A cycle and a loop aren't the same</span> .</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of nodes in the tree (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>)&nbsp;— the description of the edges of the tree.</p><p>It's guaranteed that the given graph is a tree. </p></div><div class="output-specification"><p>Output one integer&nbsp;— the maximum number of edges that Mahmoud and Ehab can add to the tree while fulfilling the conditions.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of nodes in the tree (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>)&nbsp;— the description of the edges of the tree.</p><p>It's guaranteed that the given graph is a tree. </p>

## Output

<p>Output one integer&nbsp;— the maximum number of edges that Mahmoud and Ehab can add to the tree while fulfilling the conditions.</p>





```input1
3
1 2
1 3

```




```input2
5
1 2
2 3
3 4
4 5

```




```output1
0

```




```output2
2

```



## Note

<p>Tree definition: <a href="https://en.wikipedia.org/wiki/Tree_(graph_theory)">https://en.wikipedia.org/wiki/Tree_(graph_theory)</a></p><p>Bipartite graph definition: <a href="https://en.wikipedia.org/wiki/Bipartite_graph">https://en.wikipedia.org/wiki/Bipartite_graph</a></p><p>In the first test case the only edge that can be added in such a way, that graph won't contain loops or multiple edges is <span class="tex-span">(2, 3)</span>, but adding this edge will make the graph non-bipartite so the answer is 0.</p><p>In the second test case Mahmoud and Ehab can add edges <span class="tex-span">(1, 4)</span> and <span class="tex-span">(2, 5)</span>. </p>
