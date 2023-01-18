## Description

<div><p><span class="tex-font-style-it">Tree</span> is a connected acyclic graph. Suppose you are given a tree consisting of <span class="tex-span"><i>n</i></span> vertices. The vertex of this tree is called <span class="tex-font-style-it">centroid</span> if the size of each connected component that appears if this vertex is removed from the tree doesn't exceed <img align="middle" class="tex-formula" src="file://oabgwDFN.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>You are given a tree of size <span class="tex-span"><i>n</i></span> and can perform no more than one edge replacement. <span class="tex-font-style-it">Edge replacement</span> is the operation of removing one edge from the tree (without deleting incident vertices) and inserting one new edge (without adding new vertices) in such a way that the graph remains a tree. For each vertex you have to determine if it's possible to make it centroid by performing no more than one edge replacement.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400 000</span>)&nbsp;— the number of vertices in the tree. Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains a pair of vertex indices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— endpoints of the corresponding edge.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them should be equal to <span class="tex-span">1</span> if the <span class="tex-span"><i>i</i></span>-th vertex can be made centroid by replacing no more than one edge, and should be equal to <span class="tex-span">0</span> otherwise.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400 000</span>)&nbsp;— the number of vertices in the tree. Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains a pair of vertex indices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— endpoints of the corresponding edge.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them should be equal to <span class="tex-span">1</span> if the <span class="tex-span"><i>i</i></span>-th vertex can be made centroid by replacing no more than one edge, and should be equal to <span class="tex-span">0</span> otherwise.</p>





```input1
3
1 2
2 3

```




```input2
5
1 2
1 3
1 4
1 5

```




```output1
1 1 1 

```




```output2
1 0 0 0 0 

```



## Note

<p>In the first sample each vertex can be made a centroid. For example, in order to turn vertex <span class="tex-span">1</span> to centroid one have to replace the edge <span class="tex-span">(2, 3)</span> with the edge <span class="tex-span">(1, 3)</span>.</p>
