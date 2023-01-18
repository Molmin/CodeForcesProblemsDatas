## Description

<div><p>Lech got into a tree consisting of <span class="tex-span"><i>n</i></span> vertices with a root in vertex number <span class="tex-span">1</span>. At each vertex <span class="tex-span"><i>i</i></span> written integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. He will not get out until he answers <span class="tex-span"><i>q</i></span> queries of the form <span class="tex-span"><i>u</i></span> <span class="tex-span"><i>v</i></span>. Answer for the query is maximal value <img align="middle" class="tex-formula" src="file://AmVpwkYC.png" style="max-width: 100.0%;max-height: 100.0%;"> among all vertices <span class="tex-span"><i>i</i></span> on path from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span> including <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>, where <span class="tex-span"><i>dist</i>(<i>i</i>, <i>v</i>)</span> is number of edges on path from <span class="tex-span"><i>i</i></span> to <span class="tex-span"><i>v</i></span>. Also guaranteed that vertex <span class="tex-span"><i>u</i></span> is ancestor of vertex <span class="tex-span"><i>v</i></span>. Leha's tastes are very singular: he believes that vertex is ancestor of itself.</p><p>Help Leha to get out.</p><p>The expression <img align="middle" class="tex-formula" src="file://kycwLZGv.png" style="max-width: 100.0%;max-height: 100.0%;"> means the bitwise exclusive <span class="tex-font-style-tt">OR</span> to the numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>.</p><p>Note that vertex <span class="tex-span"><i>u</i></span> is ancestor of vertex <span class="tex-span"><i>v</i></span> if vertex <span class="tex-span"><i>u</i></span> lies on the path from root to the vertex <span class="tex-span"><i>v</i></span>.</p></div><div class="input-specification"><p>First line of input data contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 150 000</span>) — number of vertices in the tree and number of queries respectively.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — numbers on vertices.</p><p>Each of next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) — description of the edges in tree.</p><p>Guaranteed that given graph is a tree.</p><p>Each of next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) — description of queries. Guaranteed that vertex <span class="tex-span"><i>u</i></span> is ancestor of vertex <span class="tex-span"><i>v</i></span>.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>q</i></span> lines — answers for a queries.</p></div>

## Input

<p>First line of input data contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 150 000</span>) — number of vertices in the tree and number of queries respectively.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — numbers on vertices.</p><p>Each of next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) — description of the edges in tree.</p><p>Guaranteed that given graph is a tree.</p><p>Each of next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) — description of queries. Guaranteed that vertex <span class="tex-span"><i>u</i></span> is ancestor of vertex <span class="tex-span"><i>v</i></span>.</p>

## Output

<p>Output <span class="tex-span"><i>q</i></span> lines — answers for a queries.</p>





```input1
5 3
0 3 2 1 4
1 2
2 3
3 4
3 5
1 4
1 5
2 4

```




```input2
5 4
1 2 3 4 5
1 2
2 3
3 4
4 5
1 5
2 5
1 4
3 3

```




```output1
3
4
3

```




```output2
5
5
4
3

```


