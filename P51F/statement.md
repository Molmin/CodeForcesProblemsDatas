## Description

<div><p>An undirected graph is called a <span class="tex-font-style-it">caterpillar</span> if it is a connected graph without cycles and it has such a path <span class="tex-span"><i>p</i></span> that any vertex is located at a distance of at most 1 from the path <span class="tex-span"><i>p</i></span>. The caterpillar can contain loops (edges from a vertex to itself) but cannot contain multiple (parallel) edges.</p><p>The picture contains an example of a caterpillar: </p><center> <img class="tex-graphics" src="file://nWuLiy20.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are given an undirected graph <span class="tex-span"><i>G</i></span>. You are allowed to do a <span class="tex-font-style-it">merging operations</span>, each such operation merges two vertices into one vertex. For that two any vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> ≠ <i>b</i></span>) are chosen. These verteces are deleted together with their edges (which are incident to at least one of the vertices <span class="tex-span"><i>a</i></span> or <span class="tex-span"><i>b</i></span>) but a new vertex <span class="tex-span"><i>w</i></span> is added together with edges <span class="tex-span">(<i>x</i>, <i>w</i>)</span> for each edge (<span class="tex-span"><i>a</i>, <i>w</i></span>) and/or (<span class="tex-span"><i>b</i>, <i>w</i></span>). If there was the edge <span class="tex-span">(<i>a</i>, <i>b</i>)</span> it transforms to the loop <span class="tex-span">(<i>w</i>, <i>w</i>)</span>. The resulting graph (after the merging operation) may contain multiple (parallel) edges between pairs of vertices and loops. Let us note that this operation decreases the number of vertices of graph by 1 but leaves the number of edges in the graph unchanged.</p><p>The merging operation can be informally described as a unity of two vertices of the graph into one with the natural transformation of the graph edges.</p><p>You may apply this operation consecutively and make the given graph to be a caterpillar. Write a program that will print the minimal number of merging operations required to make the given graph a caterpillar.</p></div><div class="input-specification"><p>The first line contains a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> represents the number of vertices in the graph and <span class="tex-span"><i>m</i></span> is the number of edges in it. Then the following <span class="tex-span"><i>m</i></span> lines contain edge descriptions, one edge description per line. Every line contains a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> which represent the indices of the vertices connected by the edge. The vertices are numbered from 1 to <span class="tex-span"><i>n</i></span>. In the given graph it will be no more than one edge between any pair of vertices. The given graph is not necessarily connected.</p></div><div class="output-specification"><p>Print the minimal required number of operations.</p></div>

## Input

<p>The first line contains a pair of integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> represents the number of vertices in the graph and <span class="tex-span"><i>m</i></span> is the number of edges in it. Then the following <span class="tex-span"><i>m</i></span> lines contain edge descriptions, one edge description per line. Every line contains a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> which represent the indices of the vertices connected by the edge. The vertices are numbered from 1 to <span class="tex-span"><i>n</i></span>. In the given graph it will be no more than one edge between any pair of vertices. The given graph is not necessarily connected.</p>

## Output

<p>Print the minimal required number of operations.</p>





```input1
4 4
1 2
2 3
3 4
4 2

```




```input2
6 3
1 2
3 4
5 6

```




```input3
7 6
1 2
2 3
1 4
4 5
1 6
6 7

```




```output1
2

```




```output2
2

```




```output3
1

```


