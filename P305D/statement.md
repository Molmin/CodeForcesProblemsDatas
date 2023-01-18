## Description

<div><p>Olya has got a directed non-weighted graph, consisting of <span class="tex-span"><i>n</i></span> vertexes and <span class="tex-span"><i>m</i></span> edges. We will consider that the graph vertexes are indexed from 1 to <span class="tex-span"><i>n</i></span> in some manner. Then for any graph edge that goes from vertex <span class="tex-span"><i>v</i></span> to vertex <span class="tex-span"><i>u</i></span> the following inequation holds: <span class="tex-span"><i>v</i> &lt; <i>u</i></span>.</p><p>Now Olya wonders, how many ways there are to add an arbitrary (possibly zero) number of edges to the graph so as the following conditions were met:</p><ol> <li> You can reach vertexes number <span class="tex-span"><i>i</i> + 1, <i>i</i> + 2, ..., <i>n</i></span> from any vertex number <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>i</i> &lt; <i>n</i>)</span>. </li><li> For any graph edge going from vertex <span class="tex-span"><i>v</i></span> to vertex <span class="tex-span"><i>u</i></span> the following inequation fulfills: <span class="tex-span"><i>v</i> &lt; <i>u</i></span>. </li><li> There is at most one edge between any two vertexes. </li><li> The shortest distance between the pair of vertexes <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(<i>i</i> &lt; <i>j</i>)</span>, for which <span class="tex-span"><i>j</i> - <i>i</i> ≤ <i>k</i></span> holds, equals <span class="tex-span"><i>j</i> - <i>i</i></span> edges. </li><li> The shortest distance between the pair of vertexes <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(<i>i</i> &lt; <i>j</i>)</span>, for which <span class="tex-span"><i>j</i> - <i>i</i> &gt; <i>k</i></span> holds, equals either <span class="tex-span"><i>j</i> - <i>i</i></span> or <span class="tex-span"><i>j</i> - <i>i</i> - <i>k</i></span> edges. </li></ol> <p>We will consider two ways <span class="tex-font-style-it">distinct</span>, if there is the pair of vertexes <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(<i>i</i> &lt; <i>j</i>)</span>, such that first resulting graph has an edge from <span class="tex-span"><i>i</i></span> to <span class="tex-span"><i>j</i></span> and the second one doesn't have it.</p><p>Help Olya. As the required number of ways can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the description of the edges of the initial graph. The <span class="tex-span"><i>i</i></span>-th line contains a pair of space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> &lt; <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the numbers of vertexes that have a directed edge from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> between them. </p><p>It is guaranteed that any pair of vertexes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> has at most one edge between them. It also is guaranteed that the graph edges are given in the order of non-decreasing <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>. If there are multiple edges going from vertex <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, then it is guaranteed that these edges are given in the order of increasing <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the description of the edges of the initial graph. The <span class="tex-span"><i>i</i></span>-th line contains a pair of space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> &lt; <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the numbers of vertexes that have a directed edge from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> between them. </p><p>It is guaranteed that any pair of vertexes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> has at most one edge between them. It also is guaranteed that the graph edges are given in the order of non-decreasing <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>. If there are multiple edges going from vertex <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, then it is guaranteed that these edges are given in the order of increasing <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
7 8 2
1 2
2 3
3 4
3 6
4 5
4 7
5 6
6 7

```




```input2
7 0 2

```




```input3
7 2 1
1 3
3 5

```




```output1
2

```




```output2
12

```




```output3
0

```



## Note

<p>In the first sample there are two ways: the first way is not to add anything, the second way is to add a single edge from vertex <span class="tex-span">2</span> to vertex <span class="tex-span">5</span>.</p>
