## Description

<div><p>Masha is fond of cacti. When she was a little girl, she decided to plant a tree. Now Masha wants to make a nice cactus out of her tree.</p><p>Recall that <span class="tex-font-style-underline">tree</span> is a connected undirected graph that has no cycles. <span class="tex-font-style-underline">Cactus</span> is a connected undirected graph such that each vertex belongs to at most one cycle.</p><p>Masha has some additional edges that she can add to a tree. For each edge she knows which vertices it would connect and the <span class="tex-font-style-underline">beauty</span> of this edge. Masha can add some of these edges to the graph if the resulting graph is a cactus. <span class="tex-font-style-underline">Beauty</span> of the resulting cactus is sum of beauties of all added edges. </p><p>Help Masha find out what maximum <span class="tex-font-style-underline">beauty</span> of the resulting cactus she can achieve.</p></div><div class="input-specification"><p>The first line of the input data contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>&nbsp;— the number of vertices in a tree, and the number of additional edges available (<span class="tex-span">3 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>; <span class="tex-span">0 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Let us describe Masha's tree. It has a root at vertex 1. The second line contains <span class="tex-span"><i>n</i> - 1</span> integers: <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, here <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— is the parent of a vertex <span class="tex-span"><i>i</i></span>&nbsp;— the first vertex on a path from the vertex <span class="tex-span"><i>i</i></span> to the root of the tree (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>).</p><p>The following <span class="tex-span"><i>m</i></span> lines contain three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— pairs of vertices to be connected by the additional edges that Masha can add to the tree and <span class="tex-font-style-underline">beauty</span> of edge (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>; <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>It is guaranteed that no additional edge coincides with the edge of the tree.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the maximum <span class="tex-font-style-underline">beauty</span> of a cactus Masha can achieve.</p></div>

## Input

<p>The first line of the input data contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>&nbsp;— the number of vertices in a tree, and the number of additional edges available (<span class="tex-span">3 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>; <span class="tex-span">0 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>Let us describe Masha's tree. It has a root at vertex 1. The second line contains <span class="tex-span"><i>n</i> - 1</span> integers: <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, here <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— is the parent of a vertex <span class="tex-span"><i>i</i></span>&nbsp;— the first vertex on a path from the vertex <span class="tex-span"><i>i</i></span> to the root of the tree (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>).</p><p>The following <span class="tex-span"><i>m</i></span> lines contain three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— pairs of vertices to be connected by the additional edges that Masha can add to the tree and <span class="tex-font-style-underline">beauty</span> of edge (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>; <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>It is guaranteed that no additional edge coincides with the edge of the tree.</p>

## Output

<p>Output one integer&nbsp;— the maximum <span class="tex-font-style-underline">beauty</span> of a cactus Masha can achieve.</p>





```input1
7 3
1 1 2 2 3 3
4 5 1
6 7 1
2 3 1

```




```output1
2

```


