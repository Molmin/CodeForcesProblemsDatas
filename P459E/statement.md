## Description

<div><p>Pashmak's homework is a problem about graphs. Although he always tries to do his homework completely, he can't solve this problem. As you know, he's really weak at graph theory; so try to help him in solving the problem.</p><p>You are given a weighted directed graph with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. You need to find a path (perhaps, non-simple) with maximum number of edges, such that the weights of the edges increase along the path. In other words, each edge of the path must have strictly greater weight than the previous edge in the path.</p><p>Help Pashmak, print the number of edges in the required path.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ <i>min</i>(<i>n</i>·(<i>n</i> - 1), 3·10<sup class="upper-index">5</sup>))</span>. Then, <span class="tex-span"><i>m</i></span> lines follows. The <span class="tex-span"><i>i</i></span>-th line contains three space separated integers: <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> which indicates that there's a directed edge with weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> from vertex <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It's guaranteed that the graph doesn't contain self-loops and multiple edges.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ <i>min</i>(<i>n</i>·(<i>n</i> - 1), 3·10<sup class="upper-index">5</sup>))</span>. Then, <span class="tex-span"><i>m</i></span> lines follows. The <span class="tex-span"><i>i</i></span>-th line contains three space separated integers: <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> which indicates that there's a directed edge with weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> from vertex <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It's guaranteed that the graph doesn't contain self-loops and multiple edges.</p>

## Output

<p>Print a single integer — the answer to the problem.</p>





```input1
3 3
1 2 1
2 3 1
3 1 1

```




```input2
3 3
1 2 1
2 3 2
3 1 3

```




```input3
6 7
1 2 1
3 2 5
2 4 2
2 5 2
2 6 9
5 4 3
4 3 4

```




```output1
1

```




```output2
3

```




```output3
6

```



## Note

<p>In the first sample the maximum trail can be any of this trails: <img align="middle" class="tex-formula" src="file://bgRw3HQz.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample the maximum trail is <img align="middle" class="tex-formula" src="file://3zXsdR7x.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the third sample the maximum trail is <img align="middle" class="tex-formula" src="file://djJVMY0t.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
