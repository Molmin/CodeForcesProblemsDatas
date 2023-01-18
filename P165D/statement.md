## Description

<div><p>Let's define a non-oriented connected graph of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>n</i> - 1</span> edges as a <span class="tex-font-style-it">beard</span>, if all of its vertices except, perhaps, one, have the degree of 2 or 1 (that is, there exists no more than one vertex, whose degree is more than two). Let us remind you that the degree of a vertex is the number of edges that connect to it. </p><p>Let each edge be either black or white. Initially all edges are black.</p><p>You are given the description of the beard graph. Your task is to analyze requests of the following types: </p><ul> <li> paint the edge number <span class="tex-span"><i>i</i></span> black. The edge number <span class="tex-span"><i>i</i></span> is the edge that has this number in the description. It is guaranteed that by the moment of this request the <span class="tex-span"><i>i</i></span>-th edge is white </li><li> paint the edge number <span class="tex-span"><i>i</i></span> white. It is guaranteed that by the moment of this request the <span class="tex-span"><i>i</i></span>-th edge is black </li><li> find the length of the shortest path going <span class="tex-font-style-bf">only along the black edges</span> between vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> or indicate that no such path exists between them (a path's length is the number of edges in it) </li></ul><p>The vertices are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and the edges are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span>.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of vertices in the graph. Next <span class="tex-span"><i>n</i> - 1</span> lines contain edges described as the numbers of vertices <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>) connected by this edge. It is guaranteed that the given graph is connected and forms a beard graph, and has no self-loops or multiple edges.</p><p>The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of requests. Next <span class="tex-span"><i>m</i></span> lines contain requests in the following form: first a line contains an integer <span class="tex-span"><i>type</i></span>, which takes values ​​from <span class="tex-span">1</span> to <span class="tex-span">3</span>, and represents the request type.</p><p>If <span class="tex-span"><i>type</i> = 1</span>, then the current request is a request to paint the edge black. In this case, in addition to number <span class="tex-span"><i>type</i></span> the line should contain integer <span class="tex-span"><i>id</i></span> (<span class="tex-span">1 ≤ <i>id</i> ≤ <i>n</i> - 1</span>), which represents the number of the edge to paint.</p><p>If <span class="tex-span"><i>type</i> = 2</span>, then the current request is a request to paint the edge white, its form is similar to the previous request.</p><p>If <span class="tex-span"><i>type</i> = 3</span>, then the current request is a request to find the distance. In this case, in addition to <span class="tex-span"><i>type</i></span>, the line should contain two integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i></span> can be equal to <span class="tex-span"><i>b</i></span>) — the numbers of vertices, the distance between which must be found.</p><p>The numbers in all lines are separated by exactly one space. The edges are numbered in the order in which they are given in the input.</p></div><div class="output-specification"><p>For each request to "find the distance between vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>" print the result. If there is no path going only along the black edges between vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, then print "-1" (without the quotes). Print the results in the order of receiving the requests, separate the numbers with spaces or line breaks.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of vertices in the graph. Next <span class="tex-span"><i>n</i> - 1</span> lines contain edges described as the numbers of vertices <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>) connected by this edge. It is guaranteed that the given graph is connected and forms a beard graph, and has no self-loops or multiple edges.</p><p>The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of requests. Next <span class="tex-span"><i>m</i></span> lines contain requests in the following form: first a line contains an integer <span class="tex-span"><i>type</i></span>, which takes values ​​from <span class="tex-span">1</span> to <span class="tex-span">3</span>, and represents the request type.</p><p>If <span class="tex-span"><i>type</i> = 1</span>, then the current request is a request to paint the edge black. In this case, in addition to number <span class="tex-span"><i>type</i></span> the line should contain integer <span class="tex-span"><i>id</i></span> (<span class="tex-span">1 ≤ <i>id</i> ≤ <i>n</i> - 1</span>), which represents the number of the edge to paint.</p><p>If <span class="tex-span"><i>type</i> = 2</span>, then the current request is a request to paint the edge white, its form is similar to the previous request.</p><p>If <span class="tex-span"><i>type</i> = 3</span>, then the current request is a request to find the distance. In this case, in addition to <span class="tex-span"><i>type</i></span>, the line should contain two integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i></span> can be equal to <span class="tex-span"><i>b</i></span>) — the numbers of vertices, the distance between which must be found.</p><p>The numbers in all lines are separated by exactly one space. The edges are numbered in the order in which they are given in the input.</p>

## Output

<p>For each request to "find the distance between vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>" print the result. If there is no path going only along the black edges between vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, then print "-1" (without the quotes). Print the results in the order of receiving the requests, separate the numbers with spaces or line breaks.</p>





```input1
3
1 2
2 3
7
3 1 2
3 1 3
3 2 3
2 2
3 1 2
3 1 3
3 2 3

```




```input2
6
1 5
6 4
2 3
3 5
5 6
6
3 3 4
2 5
3 2 6
3 1 2
2 3
3 3 1

```




```output1
1
2
1
1
-1
-1

```




```output2
3
-1
3
2

```



## Note

<p>In the first sample vertices <span class="tex-span">1</span> and <span class="tex-span">2</span> are connected with edge number <span class="tex-span">1</span>, and vertices <span class="tex-span">2</span> and <span class="tex-span">3</span> are connected with edge number <span class="tex-span">2</span>. Before the repainting edge number <span class="tex-span">2</span> each vertex is reachable from each one along the black edges. Specifically, the shortest path between <span class="tex-span">1</span> and <span class="tex-span">3</span> goes along both edges.</p><p>If we paint edge number <span class="tex-span">2</span> white, vertex <span class="tex-span">3</span> will end up cut off from other vertices, that is, no path exists from it to any other vertex along the black edges.</p>
