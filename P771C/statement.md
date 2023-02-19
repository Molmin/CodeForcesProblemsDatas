## Description

<div><p>A tree is an undirected connected graph without cycles. The distance between two vertices is the number of edges in a simple path between them.</p><p>Limak is a little polar bear. He lives in a tree that consists of <span class="tex-span"><i>n</i></span> vertices, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>.</p><p>Limak recently learned how to jump. He can jump from a vertex to any vertex within distance at most <span class="tex-span"><i>k</i></span>.</p><p>For a pair of vertices <span class="tex-span">(<i>s</i>, <i>t</i>)</span> we define <span class="tex-span"><i>f</i>(<i>s</i>, <i>t</i>)</span> as the minimum number of jumps Limak needs to get from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span>. Your task is to find the sum of <span class="tex-span"><i>f</i>(<i>s</i>, <i>t</i>)</span> over all pairs of vertices <span class="tex-span">(<i>s</i>, <i>t</i>)</span> such that <span class="tex-span"><i>s</i> &lt; <i>t</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 5</span>)&nbsp;— the number of vertices in the tree and the maximum allowed jump distance respectively.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines describe edges in the tree. The <span class="tex-span"><i>i</i></span>-th of those lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the indices on vertices connected with <span class="tex-span"><i>i</i></span>-th edge.</p><p>It's guaranteed that the given edges form a tree.</p></div><div class="output-specification"><p>Print one integer, denoting the sum of <span class="tex-span"><i>f</i>(<i>s</i>, <i>t</i>)</span> over all pairs of vertices <span class="tex-span">(<i>s</i>, <i>t</i>)</span> such that <span class="tex-span"><i>s</i> &lt; <i>t</i></span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 5</span>)&nbsp;— the number of vertices in the tree and the maximum allowed jump distance respectively.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines describe edges in the tree. The <span class="tex-span"><i>i</i></span>-th of those lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the indices on vertices connected with <span class="tex-span"><i>i</i></span>-th edge.</p><p>It's guaranteed that the given edges form a tree.</p>

## Output

<p>Print one integer, denoting the sum of <span class="tex-span"><i>f</i>(<i>s</i>, <i>t</i>)</span> over all pairs of vertices <span class="tex-span">(<i>s</i>, <i>t</i>)</span> such that <span class="tex-span"><i>s</i> &lt; <i>t</i></span>.</p>





```input1
6 2
1 2
1 3
2 4
2 5
4 6

```




```input2
13 3
1 2
3 2
4 2
5 2
3 6
10 6
6 7
6 13
5 8
5 9
9 11
11 12

```




```input3
3 5
2 1
3 1

```




```output1
20

```




```output2
114

```




```output3
3

```



## Note

<p>In the first sample, the given tree has <span class="tex-span">6</span> vertices and it's displayed on the drawing below. Limak can jump to any vertex within distance at most <span class="tex-span">2</span>. For example, from the vertex <span class="tex-span">5</span> he can jump to any of vertices: <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">4</span> (well, he can also jump to the vertex <span class="tex-span">5</span> itself).</p><center> <img class="tex-graphics" src="file://SkXzEweE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There are <img align="middle" class="tex-formula" src="file://YAP3HRtB.png" style="max-width: 100.0%;max-height: 100.0%;"> pairs of vertices <span class="tex-span">(<i>s</i>, <i>t</i>)</span> such that <span class="tex-span"><i>s</i> &lt; <i>t</i></span>. For <span class="tex-span">5</span> of those pairs Limak would need two jumps: <span class="tex-span">(1, 6), (3, 4), (3, 5), (3, 6), (5, 6)</span>. For other <span class="tex-span">10</span> pairs one jump is enough. So, the answer is <span class="tex-span">5·2 + 10·1 = 20</span>.</p><p>In the third sample, Limak can jump between every two vertices directly. There are <span class="tex-span">3</span> pairs of vertices <span class="tex-span">(<i>s</i> &lt; <i>t</i>)</span>, so the answer is <span class="tex-span">3·1 = 3</span>.</p>
