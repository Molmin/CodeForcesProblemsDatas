## Description

<div><p>You are given an undirected graph with <span class="tex-span"><i>n</i></span> vertices. There are no edge-simple cycles with the even length in it. In other words, there are no cycles of even length that pass each edge at most once. Let's enumerate vertices from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </p><p>You have to answer <span class="tex-span"><i>q</i></span> queries. Each query is described by a segment of vertices <span class="tex-span">[<i>l</i>; <i>r</i>]</span>, and you have to count the number of its subsegments <span class="tex-span">[<i>x</i>; <i>y</i>]</span> (<span class="tex-span"><i>l</i> ≤ <i>x</i> ≤ <i>y</i> ≤ <i>r</i></span>), such that if we delete all vertices except the segment of vertices <span class="tex-span">[<i>x</i>; <i>y</i>]</span> (including <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>) and edges between them, the resulting graph is bipartite.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices and the number of edges in the graph.</p><p>The next <span class="tex-span"><i>m</i></span> lines describe edges in the graph. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), denoting an edge between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that this graph does not contain edge-simple cycles of even length.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain queries. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the query parameters.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> numbers, each in new line: the <span class="tex-span"><i>i</i></span>-th of them should be the number of subsegments <span class="tex-span">[<i>x</i>; <i>y</i>]</span> (<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i> ≤ <i>y</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>), such that the graph that only includes vertices from segment <span class="tex-span">[<i>x</i>; <i>y</i>]</span> and edges between them is bipartite.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices and the number of edges in the graph.</p><p>The next <span class="tex-span"><i>m</i></span> lines describe edges in the graph. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), denoting an edge between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that this graph does not contain edge-simple cycles of even length.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain queries. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the query parameters.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> numbers, each in new line: the <span class="tex-span"><i>i</i></span>-th of them should be the number of subsegments <span class="tex-span">[<i>x</i>; <i>y</i>]</span> (<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i> ≤ <i>y</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>), such that the graph that only includes vertices from segment <span class="tex-span">[<i>x</i>; <i>y</i>]</span> and edges between them is bipartite.</p>





```input1
6 6
1 2
2 3
3 1
4 5
5 6
6 4
3
1 3
4 6
1 6

```




```input2
8 9
1 2
2 3
3 1
4 5
5 6
6 7
7 8
8 4
7 2
3
1 8
1 4
3 8

```




```output1
5
5
14

```




```output2
27
8
19

```



## Note

<p>The first example is shown on the picture below:</p><p><img class="tex-graphics" src="file://1gClQcJq.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>For the first query, all subsegments of <span class="tex-span">[1; 3]</span>, except this segment itself, are suitable.</p><p>For the first query, all subsegments of <span class="tex-span">[4; 6]</span>, except this segment itself, are suitable.</p><p>For the third query, all subsegments of <span class="tex-span">[1; 6]</span> are suitable, except <span class="tex-span">[1; 3]</span>, <span class="tex-span">[1; 4]</span>, <span class="tex-span">[1; 5]</span>, <span class="tex-span">[1; 6]</span>, <span class="tex-span">[2; 6]</span>, <span class="tex-span">[3; 6]</span>, <span class="tex-span">[4; 6]</span>.</p><p>The second example is shown on the picture below:</p><p><img class="tex-graphics" src="file://fJR8mwpF.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
