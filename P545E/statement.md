## Description

<div><p>Little girl Susie accidentally found her elder brother's notebook. She has many things to do, more important than solving problems, but she found this problem too interesting, so she wanted to know its solution and decided to ask you about it. So, the problem statement is as follows.</p><p>Let's assume that we are given a <span class="tex-font-style-bf">connected</span> weighted undirected graph <span class="tex-span"><i>G</i> = (<i>V</i>, <i>E</i>)</span> (here <span class="tex-span"><i>V</i></span> is the set of vertices, <span class="tex-span"><i>E</i></span> is the set of edges). The shortest-path tree from vertex <span class="tex-span"><i>u</i></span> is such graph <span class="tex-span"><i>G</i><sub class="lower-index">1</sub> = (<i>V</i>, <i>E</i><sub class="lower-index">1</sub>)</span> that is a tree with the set of edges <span class="tex-span"><i>E</i><sub class="lower-index">1</sub></span> that is the subset of the set of edges of the initial graph <span class="tex-span"><i>E</i></span>, and the lengths of the shortest paths from <span class="tex-span"><i>u</i></span> to any vertex to <span class="tex-span"><i>G</i></span> and to <span class="tex-span"><i>G</i><sub class="lower-index">1</sub></span> are the same. </p><p>You are given a <span class="tex-font-style-bf">connected</span> weighted undirected graph <span class="tex-span"><i>G</i></span> and vertex <span class="tex-span"><i>u</i></span>. Your task is to find the shortest-path tree of the given graph from vertex <span class="tex-span"><i>u</i></span>, the total weight of whose edges is minimum possible.</p></div><div class="input-specification"><p>The first line contains two numbers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of vertices and edges of the graph, respectively.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain three integers each, representing an edge — <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> — the numbers of vertices connected by an edge and the weight of the edge (<span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). It is guaranteed that graph is connected and that <span class="tex-font-style-bf">there is no more than one edge between any pair of vertices</span>.</p><p>The last line of the input contains integer <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>u</i> ≤ <i>n</i></span>) — the number of the start vertex.</p></div><div class="output-specification"><p>In the first line print the minimum total weight of the edges of the tree.</p><p>In the next line print the indices of the edges that are included in the tree, separated by spaces. The edges are numbered starting from <span class="tex-span">1</span> in the order they follow in the input. You may print the numbers of the edges in any order.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two numbers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of vertices and edges of the graph, respectively.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain three integers each, representing an edge — <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> — the numbers of vertices connected by an edge and the weight of the edge (<span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). It is guaranteed that graph is connected and that <span class="tex-font-style-bf">there is no more than one edge between any pair of vertices</span>.</p><p>The last line of the input contains integer <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>u</i> ≤ <i>n</i></span>) — the number of the start vertex.</p>

## Output

<p>In the first line print the minimum total weight of the edges of the tree.</p><p>In the next line print the indices of the edges that are included in the tree, separated by spaces. The edges are numbered starting from <span class="tex-span">1</span> in the order they follow in the input. You may print the numbers of the edges in any order.</p><p>If there are multiple answers, print any of them.</p>





```input1
3 3
1 2 1
2 3 1
1 3 2
3

```




```input2
4 4
1 2 1
2 3 1
3 4 1
4 1 2
4

```




```output1
2
1 2 

```




```output2
4
2 3 4 

```



## Note

<p>In the first sample there are two possible shortest path trees:</p><ul> <li> with edges <span class="tex-span">1 – 3</span> and <span class="tex-span">2 – 3</span> (the total weight is <span class="tex-span">3</span>); </li><li> with edges <span class="tex-span">1 – 2</span> and <span class="tex-span">2 – 3</span> (the total weight is <span class="tex-span">2</span>); </li></ul><p>And, for example, a tree with edges <span class="tex-span">1 – 2</span> and <span class="tex-span">1 – 3</span> won't be a shortest path tree for vertex <span class="tex-span">3</span>, because the distance from vertex <span class="tex-span">3</span> to vertex <span class="tex-span">2</span> in this tree equals <span class="tex-span">3</span>, and in the original graph it is <span class="tex-span">1</span>.</p>
