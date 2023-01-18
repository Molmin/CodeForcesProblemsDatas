## Description

<div><p>Valera had an undirected connected graph without self-loops and multiple edges consisting of <span class="tex-span"><i>n</i></span> vertices. The graph had an interesting property: there were at most <span class="tex-span"><i>k</i></span> edges adjacent to each of its vertices. For convenience, we will assume that the graph vertices were indexed by integers from 1 to <span class="tex-span"><i>n</i></span>.</p><p>One day Valera counted the shortest distances from one of the graph vertices to all other ones and wrote them out in array <span class="tex-span"><i>d</i></span>. Thus, element <span class="tex-span"><i>d</i>[<i>i</i>]</span> of the array shows the shortest distance from the vertex Valera chose to vertex number <span class="tex-span"><i>i</i></span>.</p><p>Then something irreparable terrible happened. Valera lost the initial graph. However, he still has the array <span class="tex-span"><i>d</i></span>. Help him restore the lost graph.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Number <span class="tex-span"><i>n</i></span> shows the number of vertices in the original graph. Number <span class="tex-span"><i>k</i></span> shows that at most <span class="tex-span"><i>k</i></span> edges were adjacent to each vertex in the original graph.</p><p>The second line contains space-separated integers <span class="tex-span"><i>d</i>[1], <i>d</i>[2], ..., <i>d</i>[<i>n</i>]</span> <span class="tex-span">(0 ≤ <i>d</i>[<i>i</i>] &lt; <i>n</i>)</span>. Number <span class="tex-span"><i>d</i>[<i>i</i>]</span> shows the shortest distance from the vertex Valera chose to the vertex number <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>If Valera made a mistake in his notes and the required graph doesn't exist, print in the first line number -1. Otherwise, in the first line print integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of edges in the found graph.</p><p>In each of the next <span class="tex-span"><i>m</i></span> lines print two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, denoting the edge that connects vertices with numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. The graph shouldn't contain self-loops and multiple edges. If there are multiple possible answers, print any of them.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Number <span class="tex-span"><i>n</i></span> shows the number of vertices in the original graph. Number <span class="tex-span"><i>k</i></span> shows that at most <span class="tex-span"><i>k</i></span> edges were adjacent to each vertex in the original graph.</p><p>The second line contains space-separated integers <span class="tex-span"><i>d</i>[1], <i>d</i>[2], ..., <i>d</i>[<i>n</i>]</span> <span class="tex-span">(0 ≤ <i>d</i>[<i>i</i>] &lt; <i>n</i>)</span>. Number <span class="tex-span"><i>d</i>[<i>i</i>]</span> shows the shortest distance from the vertex Valera chose to the vertex number <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>If Valera made a mistake in his notes and the required graph doesn't exist, print in the first line number -1. Otherwise, in the first line print integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of edges in the found graph.</p><p>In each of the next <span class="tex-span"><i>m</i></span> lines print two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, denoting the edge that connects vertices with numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. The graph shouldn't contain self-loops and multiple edges. If there are multiple possible answers, print any of them.</p>





```input1
3 2
0 1 1

```




```input2
4 2
2 0 1 3

```




```input3
3 1
0 0 0

```




```output1
3
1 2
1 3
3 2

```




```output2
3
1 3
1 4
2 3

```




```output3
-1

```


