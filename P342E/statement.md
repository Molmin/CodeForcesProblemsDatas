## Description

<div><p>Xenia the programmer has a tree consisting of <span class="tex-span"><i>n</i></span> nodes. We will consider the tree nodes indexed from 1 to <span class="tex-span"><i>n</i></span>. We will also consider the first node to be initially painted red, and the other nodes — to be painted blue.</p><p>The <span class="tex-font-style-it">distance</span> between two tree nodes <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> is the number of edges in the shortest path between <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span>.</p><p>Xenia needs to learn how to quickly execute queries of two types:</p><ol> <li> paint a specified blue node in red; </li><li> calculate which red node is the closest to the given one and print the shortest distance to the closest red node. </li></ol><p>Your task is to write a program which will execute the described queries.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of nodes in the tree and the number of queries. Next <span class="tex-span"><i>n</i> - 1</span> lines contain the tree edges, the <span class="tex-span"><i>i</i></span>-th line contains a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — an edge of the tree.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain queries. Each query is specified as a pair of integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2, 1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then as a reply to the query we need to paint a blue node <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> in red. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then we should reply to the query by printing the shortest distance from some red node to node <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the given graph is a tree and that all queries are correct.</p></div><div class="output-specification"><p>For each second type query print the reply in a single line.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of nodes in the tree and the number of queries. Next <span class="tex-span"><i>n</i> - 1</span> lines contain the tree edges, the <span class="tex-span"><i>i</i></span>-th line contains a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — an edge of the tree.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain queries. Each query is specified as a pair of integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2, 1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then as a reply to the query we need to paint a blue node <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> in red. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then we should reply to the query by printing the shortest distance from some red node to node <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the given graph is a tree and that all queries are correct.</p>

## Output

<p>For each second type query print the reply in a single line.</p>





```input1
5 4
1 2
2 3
2 4
4 5
2 1
2 5
1 2
2 5

```




```output1
0
3
2

```


