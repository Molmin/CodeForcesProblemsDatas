## Description

<div><p>An undirected graph is called <span class="tex-font-style-it"><span class="tex-span"><i>k</i></span>-regular</span>, if the degrees of all its vertices are equal <span class="tex-span"><i>k</i></span>. An edge of a connected graph is called a <span class="tex-font-style-it">bridge</span>, if after removing it the graph is being split into two connected components.</p><p>Build a connected undirected <span class="tex-span"><i>k</i></span>-regular graph containing at least one bridge, or else state that such graph doesn't exist.</p></div><div class="input-specification"><p>The single line of the input contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>) — the required degree of the vertices of the regular graph.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>" (without quotes), if such graph doesn't exist. </p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line and the description of any suitable graph in the next lines.</p><p>The description of the made graph must start with numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the number of vertices and edges respectively. </p><p>Each of the next <span class="tex-span"><i>m</i></span> lines must contain two integers, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>), that mean that there is an edge connecting the vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. A graph shouldn't contain multiple edges and edges that lead from a vertex to itself. A graph must be connected, the degrees of all vertices of the graph must be equal <span class="tex-span"><i>k</i></span>. At least one edge of the graph must be a bridge. You can print the edges of the graph in any order. You can print the ends of each edge in any order.</p><p>The constructed graph must contain at most <span class="tex-span">10<sup class="upper-index">6</sup></span> vertices and <span class="tex-span">10<sup class="upper-index">6</sup></span> edges (it is guaranteed that if at least one graph that meets the requirements exists, then there also exists the graph with at most <span class="tex-span">10<sup class="upper-index">6</sup></span> vertices and at most <span class="tex-span">10<sup class="upper-index">6</sup></span> edges). </p></div>

## Input

<p>The single line of the input contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>) — the required degree of the vertices of the regular graph.</p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>" (without quotes), if such graph doesn't exist. </p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line and the description of any suitable graph in the next lines.</p><p>The description of the made graph must start with numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the number of vertices and edges respectively. </p><p>Each of the next <span class="tex-span"><i>m</i></span> lines must contain two integers, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>), that mean that there is an edge connecting the vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. A graph shouldn't contain multiple edges and edges that lead from a vertex to itself. A graph must be connected, the degrees of all vertices of the graph must be equal <span class="tex-span"><i>k</i></span>. At least one edge of the graph must be a bridge. You can print the edges of the graph in any order. You can print the ends of each edge in any order.</p><p>The constructed graph must contain at most <span class="tex-span">10<sup class="upper-index">6</sup></span> vertices and <span class="tex-span">10<sup class="upper-index">6</sup></span> edges (it is guaranteed that if at least one graph that meets the requirements exists, then there also exists the graph with at most <span class="tex-span">10<sup class="upper-index">6</sup></span> vertices and at most <span class="tex-span">10<sup class="upper-index">6</sup></span> edges). </p>





```input1
1

```




```output1
YES
2 1
1 2

```



## Note

<p>In the sample from the statement there is a suitable graph consisting of two vertices, connected by a single edge.</p>
