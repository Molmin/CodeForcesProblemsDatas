## Description

<div><p>Caisa is now at home and his son has a simple task for him.</p><p>Given a rooted tree with <span class="tex-span"><i>n</i></span> vertices, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> (vertex <span class="tex-span">1</span> is the root). Each vertex of the tree has a value. You should answer <span class="tex-span"><i>q</i></span> queries. Each query is one of the following:</p><ul> <li> Format of the query is "1 <span class="tex-span"><i>v</i></span>". Let's write out the sequence of vertices along the path from the root to vertex <span class="tex-span"><i>v</i></span>: <span class="tex-span"><i>u</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>, ..., <i>u</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(<i>u</i><sub class="lower-index">1</sub> = 1;&nbsp;<i>u</i><sub class="lower-index"><i>k</i></sub> = <i>v</i>)</span>. You need to output such a vertex <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> that <span class="tex-span"><i>gcd</i>(<i>value</i>&nbsp;<i>of</i>&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub>, <i>value</i>&nbsp;<i>of</i>&nbsp;<i>v</i>) &gt; 1</span> and <span class="tex-span"><i>i</i> &lt; <i>k</i></span>. If there are several possible vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> pick the one with maximum value of <span class="tex-span"><i>i</i></span>. If there is no such vertex output <span class="tex-font-style-tt">-1</span>. </li><li> Format of the query is "2 <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>w</i></span>". You must change the value of vertex <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>w</i></span>. </li></ul><p>You are given all the queries, help Caisa to solve the problem.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">6</sup>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represent the value of node <span class="tex-span"><i>i</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>, denoting the edge of the tree between vertices <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains a query in the format that is given above. For each query the following inequalities hold: <span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>w</i> ≤ 2·10<sup class="upper-index">6</sup></span>. <span class="tex-font-style-bf">Note that</span>: there are no more than <span class="tex-span">50</span> queries that changes the value of a vertex.</p></div><div class="output-specification"><p>For each query of the first type output the result of the query.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">6</sup>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represent the value of node <span class="tex-span"><i>i</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>, denoting the edge of the tree between vertices <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains a query in the format that is given above. For each query the following inequalities hold: <span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>w</i> ≤ 2·10<sup class="upper-index">6</sup></span>. <span class="tex-font-style-bf">Note that</span>: there are no more than <span class="tex-span">50</span> queries that changes the value of a vertex.</p>

## Output

<p>For each query of the first type output the result of the query.</p>





```input1
4 6
10 8 4 3
1 2
2 3
3 4
1 1
1 2
1 3
1 4
2 1 9
1 4

```




```output1
-1
1
2
-1
1

```



## Note

<p><span class="tex-span"><i>gcd</i>(<i>x</i>, <i>y</i>)</span> is greatest common divisor of two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>.</p>
