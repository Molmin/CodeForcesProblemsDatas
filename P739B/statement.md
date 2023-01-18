## Description

<div><p>Alyona has a tree with <span class="tex-span"><i>n</i></span> vertices. The root of the tree is the vertex <span class="tex-span">1</span>. In each vertex Alyona wrote an positive integer, in the vertex <span class="tex-span"><i>i</i></span> she wrote <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Moreover, the girl wrote a positive integer to every edge of the tree (possibly, different integers on different edges).</p><p>Let's define <span class="tex-span"><i>dist</i>(<i>v</i>, <i>u</i>)</span> as the sum of the integers written on the edges of the simple path from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>.</p><p>The vertex <span class="tex-span"><i>v</i></span> controls the vertex <span class="tex-span"><i>u</i></span> (<span class="tex-span"><i>v</i> ≠ <i>u</i></span>) if and only if <span class="tex-span"><i>u</i></span> is in the subtree of <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>dist</i>(<i>v</i>, <i>u</i>) ≤ <i>a</i><sub class="lower-index"><i>u</i></sub></span>.</p><p>Alyona wants to settle in some vertex. In order to do this, she wants to know for each vertex <span class="tex-span"><i>v</i></span> what is the number of vertices <span class="tex-span"><i>u</i></span> such that <span class="tex-span"><i>v</i></span> controls <span class="tex-span"><i>u</i></span>.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the integers written in the vertices.</p><p>The next <span class="tex-span">(<i>n</i> - 1)</span> lines contain two integers each. The <span class="tex-span"><i>i</i></span>-th of these lines contains integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the parent of the <span class="tex-span">(<i>i</i> + 1)</span>-th vertex in the tree and the number written on the edge between <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span">(<i>i</i> + 1)</span>.</p><p>It is guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers&nbsp;— the <span class="tex-span"><i>i</i></span>-th of these numbers should be equal to the number of vertices that the <span class="tex-span"><i>i</i></span>-th vertex controls.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the integers written in the vertices.</p><p>The next <span class="tex-span">(<i>n</i> - 1)</span> lines contain two integers each. The <span class="tex-span"><i>i</i></span>-th of these lines contains integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the parent of the <span class="tex-span">(<i>i</i> + 1)</span>-th vertex in the tree and the number written on the edge between <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span">(<i>i</i> + 1)</span>.</p><p>It is guaranteed that the given graph is a tree.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers&nbsp;— the <span class="tex-span"><i>i</i></span>-th of these numbers should be equal to the number of vertices that the <span class="tex-span"><i>i</i></span>-th vertex controls.</p>





```input1
5
2 5 1 4 6
1 7
1 1
3 5
3 6

```




```input2
5
9 7 8 6 5
1 1
2 1
3 1
4 1

```




```output1
1 0 1 0 0

```




```output2
4 3 2 1 0

```



## Note

<p>In the example test case the vertex <span class="tex-span">1</span> controls the vertex <span class="tex-span">3</span>, the vertex <span class="tex-span">3</span> controls the vertex <span class="tex-span">5</span> (note that is doesn't mean the vertex <span class="tex-span">1</span> controls the vertex <span class="tex-span">5</span>).</p>
