## Description

<div><p>A little girl loves problems on trees very much. Here's one of them.</p><p>A tree is an undirected connected graph, not containing cycles. The degree of node <span class="tex-span"><i>x</i></span> in the tree is the number of nodes <span class="tex-span"><i>y</i></span> of the tree, such that each of them is connected with node <span class="tex-span"><i>x</i></span> by some edge of the tree. </p><p>Let's consider a tree that consists of <span class="tex-span"><i>n</i></span> nodes. We'll consider the tree's nodes indexed from 1 to <span class="tex-span"><i>n</i></span>. The cosidered tree has the following property: each node except for node number 1 has the degree of at most 2.</p><p>Initially, each node of the tree contains number 0. Your task is to quickly process the requests of two types:</p><ul> <li> Request of form: <span class="tex-span">0</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>d</i></span>. In reply to the request you should add <span class="tex-span"><i>x</i></span> to all numbers that are written in the nodes that are located at the distance of at most <span class="tex-span"><i>d</i></span> from node <span class="tex-span"><i>v</i></span>. The distance between two nodes is the number of edges on the shortest path between them. </li><li> Request of form: <span class="tex-span">1</span> <span class="tex-span"><i>v</i></span>. In reply to the request you should print the current number that is written in node <span class="tex-span"><i>v</i></span>. </li></ul></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of tree nodes and the number of requests, correspondingly.</p><p>Each of the next <span class="tex-span"><i>n</i>  -  1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>), that show that there is an edge between nodes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. Each edge's description occurs in the input exactly once. It is guaranteed that the given graph is a tree that has the property that is described in the statement.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe the requests.</p><ul> <li> The request to add has the following format: <span class="tex-span">0</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>d</i> &lt; <i>n</i></span>). </li><li> The request to print the node value has the following format: <span class="tex-span">1</span> <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>). </li></ul><p>The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>For each request to print the node value print an integer — the reply to the request.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of tree nodes and the number of requests, correspondingly.</p><p>Each of the next <span class="tex-span"><i>n</i>  -  1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>), that show that there is an edge between nodes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. Each edge's description occurs in the input exactly once. It is guaranteed that the given graph is a tree that has the property that is described in the statement.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe the requests.</p><ul> <li> The request to add has the following format: <span class="tex-span">0</span> <span class="tex-span"><i>v</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>d</i> &lt; <i>n</i></span>). </li><li> The request to print the node value has the following format: <span class="tex-span">1</span> <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>n</i></span>). </li></ul><p>The numbers in the lines are separated by single spaces.</p>

## Output

<p>For each request to print the node value print an integer — the reply to the request.</p>





```input1
3 6
1 2
1 3
0 3 1 2
0 2 3 1
0 1 5 2
1 1
1 2
1 3

```




```input2
6 11
1 2
2 5
5 4
1 6
1 3
0 3 1 3
0 3 4 5
0 2 1 4
0 1 5 5
0 4 6 2
1 1
1 2
1 3
1 4
1 5
1 6

```




```output1
9
9
6

```




```output2
11
17
11
16
17
11

```


