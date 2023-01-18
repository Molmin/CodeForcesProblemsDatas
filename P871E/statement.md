## Description

<div><p>Petya had a tree consisting of <span class="tex-span"><i>n</i></span> vertices numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Accidentally he lost his tree. </p><p>Petya remembers information about <span class="tex-span"><i>k</i></span> vertices: distances from each of them to each of the <span class="tex-span"><i>n</i></span> tree vertices.</p><p>Your task is to restore any tree that satisfies the information that Petya remembers or report that such tree doesn't exist.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 30 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(200, <i>n</i>)</span>) — the number of vertices in the tree and the number of vertices about which Petya remembers distance information.</p><p>The following <span class="tex-span"><i>k</i></span> lines contain remembered information. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>d</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>d</i><sub class="lower-index"><i>i</i>, <i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>n</i> - 1</span>), where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> — the distance to <span class="tex-span"><i>j</i></span>-th vertex from the <span class="tex-span"><i>i</i></span>-th vertex that Petya remembers.</p></div><div class="output-specification"><p>If there are no suitable trees, print <span class="tex-font-style-tt">-1</span>.</p><p>In the other case, print <span class="tex-span"><i>n</i> - 1</span> lines: each line should contain two vertices connected by edge in the required tree. You can print edges and vertices in an edge in any order. The tree vertices are enumerated from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>If there are many solutions print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 30 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(200, <i>n</i>)</span>) — the number of vertices in the tree and the number of vertices about which Petya remembers distance information.</p><p>The following <span class="tex-span"><i>k</i></span> lines contain remembered information. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>d</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>d</i><sub class="lower-index"><i>i</i>, <i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>n</i> - 1</span>), where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> — the distance to <span class="tex-span"><i>j</i></span>-th vertex from the <span class="tex-span"><i>i</i></span>-th vertex that Petya remembers.</p>

## Output

<p>If there are no suitable trees, print <span class="tex-font-style-tt">-1</span>.</p><p>In the other case, print <span class="tex-span"><i>n</i> - 1</span> lines: each line should contain two vertices connected by edge in the required tree. You can print edges and vertices in an edge in any order. The tree vertices are enumerated from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>If there are many solutions print any of them.</p>





```input1
5 2
0 1 2 3 2
2 1 0 1 2

```




```input2
3 1
1 2 1

```




```output1
2 1
3 2
4 3
5 2

```




```output2
-1

```



## Note

<p>Picture for the first sample:</p><center> <img class="tex-graphics" src="file://CSX5J4F4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
