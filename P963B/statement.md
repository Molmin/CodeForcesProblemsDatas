## Description

<div><p>You are given a tree (a graph with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>n</i> - 1</span> edges in which it's possible to reach any vertex from any other vertex using only its edges).</p><p>A vertex can be destroyed if this vertex has even degree. If you destroy a vertex, all edges connected to it are also deleted.</p><p>Destroy all vertices in the given tree or determine that it is impossible.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— number of vertices in a tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). If <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span> there is an edge between vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>If it's possible to destroy all vertices, print "<span class="tex-font-style-tt">YES</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>If it's possible to destroy all vertices, in the next <span class="tex-span"><i>n</i></span> lines print the indices of the vertices in order you destroy them. If there are multiple correct answers, print any.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— number of vertices in a tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). If <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span> there is an edge between vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that the given graph is a tree.</p>

## Output

<p>If it's possible to destroy all vertices, print "<span class="tex-font-style-tt">YES</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>If it's possible to destroy all vertices, in the next <span class="tex-span"><i>n</i></span> lines print the indices of the vertices in order you destroy them. If there are multiple correct answers, print any.</p>





```input1
5
0 1 2 1 2

```




```input2
4
0 1 2 3

```




```output1
YES
1
2
3
5
4

```




```output2
NO

```



## Note

<p>In the first example at first you have to remove the vertex with index 1 (after that, the edges (1, 2) and (1, 4) are removed), then the vertex with index 2 (and edges (2, 3) and (2, 5) are removed). After that there are no edges in the tree, so you can remove remaining vertices in any order.</p><center> <img class="tex-graphics" src="file://5iBIwEbi.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
