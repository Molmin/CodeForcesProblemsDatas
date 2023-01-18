## Description

<div><p>You are given a connected undirected graph with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. The vertices are enumerated from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </p><p>You are given <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>, each of them is between <span class="tex-span"> - <i>n</i></span> and <span class="tex-span"><i>n</i></span>, inclusive. It is also guaranteed that the parity of <span class="tex-span"><i>c</i><sub class="lower-index"><i>v</i></sub></span> equals the parity of degree of vertex <span class="tex-span"><i>v</i></span>. The degree of a vertex is the number of edges connected to it.</p><p>You are to write a weight between <span class="tex-span"> - 2·<i>n</i><sup class="upper-index">2</sup></span> and <span class="tex-span">2·<i>n</i><sup class="upper-index">2</sup></span> (inclusive) on each edge in such a way, that for each vertex <span class="tex-span"><i>v</i></span> the sum of weights on edges connected to this vertex is equal to <span class="tex-span"><i>c</i><sub class="lower-index"><i>v</i></sub></span>, or determine that this is impossible.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices and the number of edges.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - <i>n</i> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the required sum of weights of edges connected to vertex <span class="tex-span"><i>i</i></span>. It is guaranteed that the parity of <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals the parity of degree of vertex <span class="tex-span"><i>i</i></span>.</p><p>The next <span class="tex-span"><i>m</i></span> lines describe edges of the graph. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), meaning that the <span class="tex-span"><i>i</i></span>-th edge connects vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the given graph is connected and does not contain loops and multiple edges.</p></div><div class="output-specification"><p>If there is no solution, print "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" and then <span class="tex-span"><i>m</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them is the weight of the <span class="tex-span"><i>i</i></span>-th edge <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 2·<i>n</i><sup class="upper-index">2</sup> ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 2·<i>n</i><sup class="upper-index">2</sup></span>).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices and the number of edges.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - <i>n</i> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the required sum of weights of edges connected to vertex <span class="tex-span"><i>i</i></span>. It is guaranteed that the parity of <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals the parity of degree of vertex <span class="tex-span"><i>i</i></span>.</p><p>The next <span class="tex-span"><i>m</i></span> lines describe edges of the graph. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), meaning that the <span class="tex-span"><i>i</i></span>-th edge connects vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the given graph is connected and does not contain loops and multiple edges.</p>

## Output

<p>If there is no solution, print "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" and then <span class="tex-span"><i>m</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them is the weight of the <span class="tex-span"><i>i</i></span>-th edge <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 2·<i>n</i><sup class="upper-index">2</sup> ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 2·<i>n</i><sup class="upper-index">2</sup></span>).</p>





```input1
3 3
2 2 2
1 2
2 3
1 3

```




```input2
4 3
-1 0 2 1
1 2
2 3
3 4

```




```input3
6 6
3 5 5 5 1 5
1 4
3 2
4 3
4 5
3 5
5 6

```




```input4
4 4
4 4 2 4
1 2
2 3
3 4
4 1

```




```output1
YES
1
1
1

```




```output2
YES
-1
1
1

```




```output3
YES
3
5
3
-1
-3
5

```




```output4
NO
```


