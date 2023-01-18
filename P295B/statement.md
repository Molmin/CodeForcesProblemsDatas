## Description

<div><p>Greg has a weighed directed graph, consisting of <span class="tex-span"><i>n</i></span> vertices. In this graph any pair of distinct vertices has an edge between them in both directions. Greg loves playing with the graph and now he has invented a new game:</p><ul> <li> The game consists of <span class="tex-span"><i>n</i></span> steps. </li><li> On the <span class="tex-span"><i>i</i></span>-th step Greg removes vertex number <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> from the graph. As Greg removes a vertex, he also removes all the edges that go in and out of this vertex. </li><li> Before executing each step, Greg wants to know the sum of lengths of the shortest paths between all pairs of the remaining vertices. The shortest path can go through any remaining vertex. In other words, if we assume that <span class="tex-span"><i>d</i>(<i>i</i>, <i>v</i>, <i>u</i>)</span> is the shortest path between vertices <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> in the graph that formed before deleting vertex <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, then Greg wants to know the value of the following sum: <img align="middle" class="tex-formula" src="file://1xM5IIPT.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul><p>Help Greg, print the value of the required sum before each step.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 500)</span> — the number of vertices in the graph.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> integers each — the graph adjacency matrix: the <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th line <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">5</sup>, <i>a</i><sub class="lower-index"><i>ii</i></sub> = 0)</span> represents the weight of the edge that goes from vertex <span class="tex-span"><i>i</i></span> to vertex <span class="tex-span"><i>j</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> distinct integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the vertices that Greg deletes.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers — the <span class="tex-span"><i>i</i></span>-th number equals the required sum before the <span class="tex-span"><i>i</i></span>-th step.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams of the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 500)</span> — the number of vertices in the graph.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> integers each — the graph adjacency matrix: the <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th line <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">5</sup>, <i>a</i><sub class="lower-index"><i>ii</i></sub> = 0)</span> represents the weight of the edge that goes from vertex <span class="tex-span"><i>i</i></span> to vertex <span class="tex-span"><i>j</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> distinct integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the vertices that Greg deletes.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers — the <span class="tex-span"><i>i</i></span>-th number equals the required sum before the <span class="tex-span"><i>i</i></span>-th step.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams of the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
1
0
1

```




```input2
2
0 5
4 0
1 2

```




```input3
4
0 3 1 1
6 0 400 1
2 4 0 1
1 1 1 0
4 1 2 3

```




```output1
0
```




```output2
9 0
```




```output3
17 23 404 0
```


