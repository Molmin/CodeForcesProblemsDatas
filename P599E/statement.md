## Description

<div><p><span class="tex-font-style-it">Rooted tree</span> is a connected graph without any simple cycles with one vertex selected as a root. In this problem the vertex number <span class="tex-span">1</span> will always serve as a root.</p><p><span class="tex-font-style-it">Lowest common ancestor</span> of two vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> is the farthest from the root vertex that lies on both the path from <span class="tex-span"><i>u</i></span> to the root and on path from <span class="tex-span"><i>v</i></span> to the root. We will denote it as <span class="tex-span"><i>LCA</i>(<i>u</i>, <i>v</i>)</span>.</p><p>Sandy had a rooted tree consisting of <span class="tex-span"><i>n</i></span> vertices that she used to store her nuts. Unfortunately, the underwater storm broke her tree and she doesn't remember all it's edges. She only managed to restore <span class="tex-span"><i>m</i></span> edges of the initial tree and <span class="tex-span"><i>q</i></span> triples <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, for which she supposes <span class="tex-span"><i>LCA</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>) = <i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Help Sandy count the number of trees of size <span class="tex-span"><i>n</i></span> with vertex <span class="tex-span">1</span> as a root, that match all the information she remembered. If she made a mess and there are no such trees then print <span class="tex-span">0</span>. Two rooted trees are considered to be distinct if there exists an edge that occur in one of them and doesn't occur in the other one.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 13, 0 ≤ <i>m</i> &lt; <i>n</i>, 0 ≤ <i>q</i> ≤ 100</span>)&nbsp;— the number of vertices, the number of edges and <span class="tex-span"><i>LCA</i></span> triples remembered by Sandy respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the numbers of vertices connected by the <span class="tex-span"><i>i</i></span>-th edge. It's guaranteed that this set of edges is a subset of edges of some tree.</p><p>The last <span class="tex-span"><i>q</i></span> lines contain the triplets of numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. Each of these triples define <span class="tex-span"><i>LCA</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>) = <i>c</i><sub class="lower-index"><i>i</i></sub></span>. It's <span class="tex-font-style-bf">not guaranteed</span> that there exists a tree that satisfy all the given <span class="tex-span"><i>LCA</i></span> conditions.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of trees of size <span class="tex-span"><i>n</i></span> that satisfy all the conditions.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 13, 0 ≤ <i>m</i> &lt; <i>n</i>, 0 ≤ <i>q</i> ≤ 100</span>)&nbsp;— the number of vertices, the number of edges and <span class="tex-span"><i>LCA</i></span> triples remembered by Sandy respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the numbers of vertices connected by the <span class="tex-span"><i>i</i></span>-th edge. It's guaranteed that this set of edges is a subset of edges of some tree.</p><p>The last <span class="tex-span"><i>q</i></span> lines contain the triplets of numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. Each of these triples define <span class="tex-span"><i>LCA</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>) = <i>c</i><sub class="lower-index"><i>i</i></sub></span>. It's <span class="tex-font-style-bf">not guaranteed</span> that there exists a tree that satisfy all the given <span class="tex-span"><i>LCA</i></span> conditions.</p>

## Output

<p>Print a single integer&nbsp;— the number of trees of size <span class="tex-span"><i>n</i></span> that satisfy all the conditions.</p>





```input1
4 0 0

```




```input2
4 0 1
3 4 2

```




```input3
3 1 0
1 2

```




```input4
3 0 2
2 3 2
2 3 1

```




```input5
4 1 2
1 2
2 2 2
3 4 2

```




```output1
16

```




```output2
1

```




```output3
2

```




```output4
0

```




```output5
1

```



## Note

<p>In the second sample correct answer looks like this:</p><center> <img class="tex-graphics" height="265px" src="file://Z8DODVaD.png" style="max-width: 100.0%;max-height: 100.0%;" width="227px"> </center><p>In the third sample there are two possible trees:</p><center> <img class="tex-graphics" height="340px" src="file://wovHpTOF.png" style="max-width: 100.0%;max-height: 100.0%;" width="113px"> </center><center> <img class="tex-graphics" height="265px" src="file://EkortgFM.png" style="max-width: 100.0%;max-height: 100.0%;" width="227px"> </center><p>In the fourth sample the answer is <span class="tex-span">0</span> because the information about <span class="tex-span"><i>LCA</i></span> is inconsistent.</p>
