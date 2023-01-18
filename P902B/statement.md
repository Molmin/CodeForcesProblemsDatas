## Description

<div><p>You are given a rooted tree with <span class="tex-span"><i>n</i></span> vertices. The vertices are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, the root is the vertex number <span class="tex-span">1</span>.</p><p>Each vertex has a color, let's denote the color of vertex <span class="tex-span"><i>v</i></span> by <span class="tex-span"><i>c</i><sub class="lower-index"><i>v</i></sub></span>. Initially <span class="tex-span"><i>c</i><sub class="lower-index"><i>v</i></sub> = 0</span>.</p><p>You have to color the tree into the given colors using the smallest possible number of steps. On each step you can choose a vertex <span class="tex-span"><i>v</i></span> and a color <span class="tex-span"><i>x</i></span>, and then color all vectices in the subtree of <span class="tex-span"><i>v</i></span> (including <span class="tex-span"><i>v</i></span> itself) in color <span class="tex-span"><i>x</i></span>. In other words, for every vertex <span class="tex-span"><i>u</i></span>, such that the path from root to <span class="tex-span"><i>u</i></span> passes through <span class="tex-span"><i>v</i></span>, set <span class="tex-span"><i>c</i><sub class="lower-index"><i>u</i></sub> = <i>x</i></span>.</p><p>It is guaranteed that you have to color each vertex in a color different from <span class="tex-span">0</span>.</p><p>You can learn what a rooted tree is using the link: <a href="https://en.wikipedia.org/wiki/Tree_(graph_theory)">https://en.wikipedia.org/wiki/Tree_(graph_theory)</a>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> means that there is an edge between vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the color you should color the <span class="tex-span"><i>i</i></span>-th vertex into.</p><p>It is guaranteed that the given graph is a tree. </p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of steps you have to perform to color the tree into given colors.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> means that there is an edge between vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the color you should color the <span class="tex-span"><i>i</i></span>-th vertex into.</p><p>It is guaranteed that the given graph is a tree. </p>

## Output

<p>Print a single integer&nbsp;— the minimum number of steps you have to perform to color the tree into given colors.</p>





```input1
6
1 2 2 1 5
2 1 1 1 1 1

```




```input2
7
1 1 2 3 1 4
3 3 1 1 1 2 3

```




```output1
3

```




```output2
5

```



## Note

<p>The tree from the first sample is shown on the picture (numbers are vetices' indices):</p><p><img class="tex-graphics" src="file://Jrq3Uy29.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>On first step we color all vertices in the subtree of vertex <span class="tex-span">1</span> into color <span class="tex-span">2</span> (numbers are colors):</p><p><img class="tex-graphics" src="file://JRuCbcWw.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>On seond step we color all vertices in the subtree of vertex <span class="tex-span">5</span> into color <span class="tex-span">1</span>:</p><p><img class="tex-graphics" src="file://EiiQZUyV.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>On third step we color all vertices in the subtree of vertex <span class="tex-span">2</span> into color <span class="tex-span">1</span>:</p><p><img class="tex-graphics" src="file://XaTbrPqf.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The tree from the second sample is shown on the picture (numbers are vetices' indices):</p><p><img class="tex-graphics" src="file://RgndfIHR.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>On first step we color all vertices in the subtree of vertex <span class="tex-span">1</span> into color <span class="tex-span">3</span> (numbers are colors):</p><p><img class="tex-graphics" src="file://IjSkSS9m.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>On second step we color all vertices in the subtree of vertex <span class="tex-span">3</span> into color <span class="tex-span">1</span>:</p><p><img class="tex-graphics" src="file://I1v5NISL.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>On third step we color all vertices in the subtree of vertex <span class="tex-span">6</span> into color <span class="tex-span">2</span>:</p><p><img class="tex-graphics" src="file://f6YWoUi5.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>On fourth step we color all vertices in the subtree of vertex <span class="tex-span">4</span> into color <span class="tex-span">1</span>:</p><p><img class="tex-graphics" src="file://WwFhB3Is.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>On fith step we color all vertices in the subtree of vertex <span class="tex-span">7</span> into color <span class="tex-span">3</span>:</p><p><img class="tex-graphics" src="file://CHMLJQeC.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
