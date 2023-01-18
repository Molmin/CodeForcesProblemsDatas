## Description

<div><p>You are given a tree consisting of <span class="tex-span"><i>n</i></span> vertices (numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>). Initially all vertices are white. You have to process <span class="tex-span"><i>q</i></span> queries of two different types:</p><ol> <li> <span class="tex-span">1</span> <span class="tex-span"><i>x</i></span> — change the color of vertex <span class="tex-span"><i>x</i></span> to black. It is guaranteed that the first query will be of this type. </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>x</i></span> — for the vertex <span class="tex-span"><i>x</i></span>, find the minimum index <span class="tex-span"><i>y</i></span> such that the vertex with index <span class="tex-span"><i>y</i></span> belongs to the simple path from <span class="tex-span"><i>x</i></span> to some black vertex (a simple path never visits any vertex more than once). </li></ol><p>For each query of type <span class="tex-span">2</span> print the answer to it.</p><p><span class="tex-font-style-bf">Note that the queries are given in modified way</span>.</p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow, each line containing two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and representing the edge between vertices <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that these edges form a tree.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. Each line contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the type of <span class="tex-span"><i>i</i></span>th query, and <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> can be used to restore <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> for this query in this way: you have to keep track of the answer to the last query of type <span class="tex-span">2</span> (let's call this answer <span class="tex-span"><i>last</i></span>, and initially <span class="tex-span"><i>last</i> = 0</span>); then <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = (<i>z</i><sub class="lower-index"><i>i</i></sub> + <i>last</i>) <i>mod</i> <i>n</i> + 1</span>.</p><p>It is guaranteed that the first query is of type <span class="tex-span">1</span>, and there is at least one query of type <span class="tex-span">2</span>.</p></div><div class="output-specification"><p>For each query of type <span class="tex-span">2</span> output the answer to it.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow, each line containing two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and representing the edge between vertices <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that these edges form a tree.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow. Each line contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the type of <span class="tex-span"><i>i</i></span>th query, and <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> can be used to restore <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> for this query in this way: you have to keep track of the answer to the last query of type <span class="tex-span">2</span> (let's call this answer <span class="tex-span"><i>last</i></span>, and initially <span class="tex-span"><i>last</i> = 0</span>); then <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = (<i>z</i><sub class="lower-index"><i>i</i></sub> + <i>last</i>) <i>mod</i> <i>n</i> + 1</span>.</p><p>It is guaranteed that the first query is of type <span class="tex-span">1</span>, and there is at least one query of type <span class="tex-span">2</span>.</p>

## Output

<p>For each query of type <span class="tex-span">2</span> output the answer to it.</p>





```input1
4 6
1 2
2 3
3 4
1 2
1 2
2 2
1 3
2 2
2 2

```




```output1
3
2
1

```


