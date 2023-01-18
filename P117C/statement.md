## Description

<div><p>A <span class="tex-font-style-underline">tournament</span> is a directed graph without self-loops in which every pair of vertexes is connected by exactly one directed edge. That is, for any two vertexes <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span"><i>u</i> ≠ <i>v</i></span>) exists either an edge going from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span>, or an edge from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>.</p><p>You are given a tournament consisting of <span class="tex-span"><i>n</i></span> vertexes. Your task is to find there a cycle of length three.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>). Next <span class="tex-span"><i>n</i></span> lines contain the adjacency matrix <span class="tex-span"><i>A</i></span> of the graph (without spaces). <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 1</span> if the graph has an edge going from vertex <span class="tex-span"><i>i</i></span> to vertex <span class="tex-span"><i>j</i></span>, otherwise <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>. <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> stands for the <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th line.</p><p>It is guaranteed that the given graph is a tournament, that is, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0, <i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≠ <i>A</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>, <i>i</i> ≠ <i>j</i>)</span>.</p></div><div class="output-specification"><p>Print three distinct vertexes of the graph <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), such that <span class="tex-span"><i>A</i><sub class="lower-index"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub></sub> = <i>A</i><sub class="lower-index"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub></sub> = <i>A</i><sub class="lower-index"><i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">1</sub></sub> = 1</span>, or "<span class="tex-font-style-tt">-1</span>", if a cycle whose length equals three does not exist. </p><p>If there are several solutions, print any of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>). Next <span class="tex-span"><i>n</i></span> lines contain the adjacency matrix <span class="tex-span"><i>A</i></span> of the graph (without spaces). <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 1</span> if the graph has an edge going from vertex <span class="tex-span"><i>i</i></span> to vertex <span class="tex-span"><i>j</i></span>, otherwise <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>. <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> stands for the <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th line.</p><p>It is guaranteed that the given graph is a tournament, that is, <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0, <i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≠ <i>A</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>, <i>i</i> ≠ <i>j</i>)</span>.</p>

## Output

<p>Print three distinct vertexes of the graph <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), such that <span class="tex-span"><i>A</i><sub class="lower-index"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub></sub> = <i>A</i><sub class="lower-index"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub></sub> = <i>A</i><sub class="lower-index"><i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">1</sub></sub> = 1</span>, or "<span class="tex-font-style-tt">-1</span>", if a cycle whose length equals three does not exist. </p><p>If there are several solutions, print any of them.</p>





```input1
5
00100
10000
01001
11101
11000

```




```input2
5
01111
00000
01000
01100
01110

```




```output1
1 3 2
```




```output2
-1

```


