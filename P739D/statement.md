## Description

<div><p>Functional graph is a directed graph in which all vertices have outdegree equal to <span class="tex-span">1</span>. Loops are allowed.</p><p>Some vertices of a functional graph lay on a cycle. From the others we can come to a cycle by making a finite number of steps along the edges (we consider only finite functional graphs in this problem).</p><p>Let's compute two values for each vertex. <span class="tex-span"><i>precycle</i><sub class="lower-index"><i>i</i></sub></span> is the amount of edges we should pass to get to a vertex which is a part of some cycle (zero, if <span class="tex-span"><i>i</i></span> itself lies on a cycle), <span class="tex-span"><i>cycle</i><sub class="lower-index"><i>i</i></sub></span> is the length of the cycle we get to.</p><p>You are given the information about these values for some functional graph. For each vertex you know the values <span class="tex-span"><i>precycle</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>cycle</i><sub class="lower-index"><i>i</i></sub></span>, however, instead of some values there can be the question mark. It means that these values are unknown.</p><p>Build any functional graph that suits the description or determine that there is no such graph.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>)&nbsp;— the number of vertices in the graph.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contain two integers&nbsp;— <span class="tex-span"><i>precycle</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>precycle</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) and <span class="tex-span"><i>cycle</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>cycle</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). There could be question marks instead of some of these values.</p></div><div class="output-specification"><p>In case there is no solution, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, print <span class="tex-span"><i>n</i></span> integers. <span class="tex-span"><i>i</i></span>-th of them is the number of vertex to which the edge form the <span class="tex-span"><i>i</i></span>-th vertex go.</p><p>The vertices should be in the same order as they go in input data.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>)&nbsp;— the number of vertices in the graph.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contain two integers&nbsp;— <span class="tex-span"><i>precycle</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>precycle</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) and <span class="tex-span"><i>cycle</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>cycle</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). There could be question marks instead of some of these values.</p>

## Output

<p>In case there is no solution, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, print <span class="tex-span"><i>n</i></span> integers. <span class="tex-span"><i>i</i></span>-th of them is the number of vertex to which the edge form the <span class="tex-span"><i>i</i></span>-th vertex go.</p><p>The vertices should be in the same order as they go in input data.</p><p>If there are multiple solutions, print any of them.</p>





```input1
3
0 3
0 3
? ?

```




```input2
5
3 2
? ?
? ?
? ?
? ?

```




```input3
8
? 3
? ?
0 2
0 2
0 3
0 3
0 3
3 3

```




```input4
1
? ?

```




```input5
6
0 3
0 3
0 3
0 3
0 3
0 3

```




```input6
2
1 1
1 1

```




```output1
2 3 1 

```




```output2
5 3 2 2 4 

```




```output3
5 1 4 3 6 7 5 2 

```




```output4
1 

```




```output5
2 3 1 5 6 4 

```




```output6
-1

```


