## Description

<div><p>Mad scientist Mike has constructed a rooted tree, which consists of <span class="tex-span"><i>n</i></span> vertices. Each vertex is a reservoir which can be either empty or filled with water.</p><p>The vertices of the tree are numbered from 1 to <span class="tex-span"><i>n</i></span> with the root at vertex 1. For each vertex, the reservoirs of its children are located below the reservoir of this vertex, and the vertex is connected with each of the children by a pipe through which water can flow downwards.</p><p>Mike wants to do the following operations with the tree: </p><ol> <li> Fill vertex <span class="tex-span"><i>v</i></span> with water. Then <span class="tex-span"><i>v</i></span> and all its children are filled with water. </li><li> Empty vertex <span class="tex-span"><i>v</i></span>. Then <span class="tex-span"><i>v</i></span> and all its ancestors are emptied. </li><li> Determine whether vertex <span class="tex-span"><i>v</i></span> is filled with water at the moment. </li></ol> Initially all vertices of the tree are empty.<p>Mike has already compiled a full list of operations that he wants to perform in order. Before experimenting with the tree Mike decided to run the list through a simulation. Help Mike determine what results will he get after performing all the operations.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500000</span>) — the number of vertices in the tree. Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — the edges of the tree.</p><p>The next line contains a number <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 500000</span>) — the number of operations to perform. Each of the following <span class="tex-span"><i>q</i></span> lines contains two space-separated numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>), <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the operation type (according to the numbering given in the statement), and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> is the vertex on which the operation is performed.</p><p>It is guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>For each type 3 operation print 1 on a separate line if the vertex is full, and 0 if the vertex is empty. Print the answers to queries in the order in which the queries are given in the input.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500000</span>) — the number of vertices in the tree. Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — the edges of the tree.</p><p>The next line contains a number <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 500000</span>) — the number of operations to perform. Each of the following <span class="tex-span"><i>q</i></span> lines contains two space-separated numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>), <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the operation type (according to the numbering given in the statement), and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> is the vertex on which the operation is performed.</p><p>It is guaranteed that the given graph is a tree.</p>

## Output

<p>For each type 3 operation print 1 on a separate line if the vertex is full, and 0 if the vertex is empty. Print the answers to queries in the order in which the queries are given in the input.</p>





```input1
5
1 2
5 1
2 3
4 2
12
1 1
2 3
3 1
3 2
3 3
3 4
1 2
2 4
3 1
3 3
3 4
3 5

```




```output1
0
0
0
1
0
1
0
1

```


