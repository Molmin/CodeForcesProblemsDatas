## Description

<div><p>A <span class="tex-font-style-it">tree</span> is a connected graph that doesn't contain any cycles.</p><p>The <span class="tex-font-style-it">distance</span> between two vertices of a tree is the length (in edges) of the shortest path between these vertices.</p><p>You are given a tree with <span class="tex-span"><i>n</i></span> vertices and a positive number <span class="tex-span"><i>k</i></span>. Find the number of distinct pairs of the vertices which have a distance of exactly <span class="tex-span"><i>k</i></span> between them. Note that pairs (<span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>u</i></span>) and (<span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span>) are considered to be the same pair.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 500</span>) — the number of vertices and the required distance between the vertices.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe the edges as "<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes) (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the vertices connected by the <span class="tex-span"><i>i</i></span>-th edge. All given edges are different.</p></div><div class="output-specification"><p>Print a single integer — the number of distinct pairs of the tree's vertices which have a distance of exactly <span class="tex-span"><i>k</i></span> between them.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 500</span>) — the number of vertices and the required distance between the vertices.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe the edges as "<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes) (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the vertices connected by the <span class="tex-span"><i>i</i></span>-th edge. All given edges are different.</p>

## Output

<p>Print a single integer — the number of distinct pairs of the tree's vertices which have a distance of exactly <span class="tex-span"><i>k</i></span> between them.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5 2
1 2
2 3
3 4
2 5

```




```input2
5 3
1 2
2 3
3 4
4 5

```




```output1
4

```




```output2
2

```



## Note

<p>In the first sample the pairs of vertexes at distance 2 from each other are (1, 3), (1, 5), (3, 5) and (2, 4).</p>
