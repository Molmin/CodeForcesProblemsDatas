## Description

<div><p>You are given an undirected graph that consists of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. Initially, each edge is colored either red or blue. Each turn a player picks a single vertex and switches the color of <span class="tex-font-style-bf">all</span> edges incident to it. That is, all red edges with an endpoint in this vertex change the color to blue, while all blue edges with an endpoint in this vertex change the color to red.</p><p>Find the minimum possible number of moves required to make the colors of all edges equal.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the number of vertices and edges, respectively.</p><p>The following <span class="tex-span"><i>m</i></span> lines provide the description of the edges, as the <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the indices of the vertices connected by the <span class="tex-span"><i>i</i></span>-th edge, and a character <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://rDSgQwkj.png" style="max-width: 100.0%;max-height: 100.0%;">) providing the initial color of this edge. If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals '<span class="tex-font-style-tt">R</span>', then this edge is initially colored red. Otherwise, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is equal to '<span class="tex-font-style-tt">B</span>' and this edge is initially colored blue. It's guaranteed that there are no self-loops and multiple edges.</p></div><div class="output-specification"><p>If there is no way to make the colors of all edges equal output <span class="tex-span"> - 1</span> in the only line of the output. Otherwise first output <span class="tex-span"><i>k</i></span>&nbsp;— the minimum number of moves required to achieve the goal, then output <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the index of the vertex that should be used at the <span class="tex-span"><i>i</i></span>-th move.</p><p>If there are multiple optimal sequences of moves, output any of them.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the number of vertices and edges, respectively.</p><p>The following <span class="tex-span"><i>m</i></span> lines provide the description of the edges, as the <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the indices of the vertices connected by the <span class="tex-span"><i>i</i></span>-th edge, and a character <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://rDSgQwkj.png" style="max-width: 100.0%;max-height: 100.0%;">) providing the initial color of this edge. If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals '<span class="tex-font-style-tt">R</span>', then this edge is initially colored red. Otherwise, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is equal to '<span class="tex-font-style-tt">B</span>' and this edge is initially colored blue. It's guaranteed that there are no self-loops and multiple edges.</p>

## Output

<p>If there is no way to make the colors of all edges equal output <span class="tex-span"> - 1</span> in the only line of the output. Otherwise first output <span class="tex-span"><i>k</i></span>&nbsp;— the minimum number of moves required to achieve the goal, then output <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the index of the vertex that should be used at the <span class="tex-span"><i>i</i></span>-th move.</p><p>If there are multiple optimal sequences of moves, output any of them.</p>





```input1
3 3
1 2 B
3 1 R
3 2 B

```




```input2
6 5
1 3 R
2 3 R
3 4 B
4 5 R
4 6 R

```




```input3
4 5
1 2 R
1 3 R
2 3 B
3 4 B
1 4 B

```




```output1
1
2 

```




```output2
2
3 4 

```




```output3
-1

```


