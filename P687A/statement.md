## Description

<div><p>Recently, Pari and Arya did some research about NP-Hard problems and they found the <span class="tex-font-style-underline">minimum vertex cover</span> problem very interesting.</p><p>Suppose the graph <span class="tex-span"><i>G</i></span> is given. Subset <span class="tex-span"><i>A</i></span> of its vertices is called a <span class="tex-font-style-underline">vertex cover</span> of this graph, if for each edge <span class="tex-span"><i>uv</i></span> there is at least one endpoint of it in this set, i.e. <img align="middle" class="tex-formula" src="file://f2DlRNjy.png" style="max-width: 100.0%;max-height: 100.0%;"> or <img align="middle" class="tex-formula" src="file://I3r9268C.png" style="max-width: 100.0%;max-height: 100.0%;"> (or both).</p><p>Pari and Arya have won a great undirected graph as an award in a team contest. Now they have to split it in two parts, but both of them want their parts of the graph to be a vertex cover.</p><p>They have agreed to give you their graph and you need to find two <span class="tex-font-style-bf">disjoint</span> subsets of its vertices <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>, such that both <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> are vertex cover or claim it's impossible. Each vertex should be given to no more than one of the friends (or you can even keep it for yourself).</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of vertices and the number of edges in the prize graph, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤  <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub>  ≤  <i>n</i></span>), denoting an undirected edge between <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed the graph won't contain any self-loops or multiple edges.</p></div><div class="output-specification"><p>If it's impossible to split the graph between Pari and Arya as they expect, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p><p>If there are two disjoint sets of vertices, such that both sets are vertex cover, print their descriptions. Each description must contain two lines. The first line contains a single integer <span class="tex-span"><i>k</i></span> denoting the number of vertices in that vertex cover, and the second line contains <span class="tex-span"><i>k</i></span> integers&nbsp;— the indices of vertices. Note that because of <span class="tex-span"><i>m</i> ≥ 1</span>, vertex cover cannot be empty.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of vertices and the number of edges in the prize graph, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤  <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub>  ≤  <i>n</i></span>), denoting an undirected edge between <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed the graph won't contain any self-loops or multiple edges.</p>

## Output

<p>If it's impossible to split the graph between Pari and Arya as they expect, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p><p>If there are two disjoint sets of vertices, such that both sets are vertex cover, print their descriptions. Each description must contain two lines. The first line contains a single integer <span class="tex-span"><i>k</i></span> denoting the number of vertices in that vertex cover, and the second line contains <span class="tex-span"><i>k</i></span> integers&nbsp;— the indices of vertices. Note that because of <span class="tex-span"><i>m</i> ≥ 1</span>, vertex cover cannot be empty.</p>





```input1
4 2
1 2
2 3

```




```input2
3 3
1 2
2 3
1 3

```




```output1
1
2 
2
1 3 

```




```output2
-1

```



## Note

<p>In the first sample, you can give the vertex number <span class="tex-span">2</span> to Arya and vertices numbered <span class="tex-span">1</span> and <span class="tex-span">3</span> to Pari and keep vertex number <span class="tex-span">4</span> for yourself (or give it someone, if you wish).</p><p>In the second sample, there is no way to satisfy both Pari and Arya.</p>
