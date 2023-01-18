## Description

<div><p>You are given a rooted tree consisting of <span class="tex-span"><i>n</i></span> vertices. Each vertex has a number written on it; number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is written on vertex <span class="tex-span"><i>i</i></span>.</p><p>Let's denote <span class="tex-span"><i>d</i>(<i>i</i>, <i>j</i>)</span> as the distance between vertices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> in the tree (that is, the number of edges in the shortest path from <span class="tex-span"><i>i</i></span> to <span class="tex-span"><i>j</i></span>). Also let's denote the <span class="tex-font-style-it"><span class="tex-span"><i>k</i></span>-blocked subtree</span> of vertex <span class="tex-span"><i>x</i></span> as the set of vertices <span class="tex-span"><i>y</i></span> such that both these conditions are met:</p><ul> <li> <span class="tex-span"><i>x</i></span> is an ancestor of <span class="tex-span"><i>y</i></span> (every vertex is an ancestor of itself); </li><li> <span class="tex-span"><i>d</i>(<i>x</i>, <i>y</i>) ≤ <i>k</i></span>. </li></ul><p>You are given <span class="tex-span"><i>m</i></span> queries to the tree. <span class="tex-span"><i>i</i></span>-th query is represented by two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, and the answer to this query is the minimum value of <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> among such vertices <span class="tex-span"><i>j</i></span> such that <span class="tex-span"><i>j</i></span> belongs to <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>-blocked subtree of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Write a program that would process these queries quickly!</p><p><span class="tex-font-style-bf">Note that the queries are given in a modified way</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i> ≤ 100000</span>) — the number of vertices in the tree and the index of the root, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the numbers written on the vertices.</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow, each containing two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>) and representing an edge between vertices <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. It is guaranteed that these edges form a tree.</p><p>Next line contains one integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of queries to process.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line containing two numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>, which can be used to restore <span class="tex-span"><i>i</i></span>-th query (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p><p><span class="tex-span"><i>i</i></span>-th query can be restored as follows:</p><p>Let <span class="tex-span"><i>last</i></span> be the answer for previous query (or <span class="tex-span">0</span> if <span class="tex-span"><i>i</i> = 1</span>). Then <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = ((<i>p</i><sub class="lower-index"><i>i</i></sub> + <i>last</i>) <i>mod</i> <i>n</i>) + 1</span>, and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub> = (<i>q</i><sub class="lower-index"><i>i</i></sub> + <i>last</i>) <i>mod</i> <i>n</i></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers. <span class="tex-span"><i>i</i></span>-th of them has to be equal to the answer to <span class="tex-span"><i>i</i></span>-th query.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i> ≤ 100000</span>) — the number of vertices in the tree and the index of the root, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the numbers written on the vertices.</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow, each containing two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>) and representing an edge between vertices <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. It is guaranteed that these edges form a tree.</p><p>Next line contains one integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of queries to process.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line containing two numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>, which can be used to restore <span class="tex-span"><i>i</i></span>-th query (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p><p><span class="tex-span"><i>i</i></span>-th query can be restored as follows:</p><p>Let <span class="tex-span"><i>last</i></span> be the answer for previous query (or <span class="tex-span">0</span> if <span class="tex-span"><i>i</i> = 1</span>). Then <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = ((<i>p</i><sub class="lower-index"><i>i</i></sub> + <i>last</i>) <i>mod</i> <i>n</i>) + 1</span>, and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub> = (<i>q</i><sub class="lower-index"><i>i</i></sub> + <i>last</i>) <i>mod</i> <i>n</i></span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers. <span class="tex-span"><i>i</i></span>-th of them has to be equal to the answer to <span class="tex-span"><i>i</i></span>-th query.</p>





```input1
5 2
1 3 2 3 5
2 3
5 1
3 4
4 1
2
1 2
2 3

```




```output1
2
5

```


