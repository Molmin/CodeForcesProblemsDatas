## Description

<div><p>Sloth is bad, mkay? So we decided to prepare a problem to punish lazy guys.</p><p>You are given a tree, you should count the number of ways to remove an edge from it and then add an edge to it such that the final graph is a tree and has a perfect matching. Two ways of this operation are considered different if their removed edges or their added edges aren't the same. The removed edge and the added edge can be equal.</p><p>A perfect matching is a subset of edges such that each vertex is an endpoint of exactly one of these edges.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— the endpoints of one edge. It's guaranteed that the graph is a tree.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the answer to the problem.</p></div>

## Input

<p>The first line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— the endpoints of one edge. It's guaranteed that the graph is a tree.</p>

## Output

<p>Output a single integer&nbsp;— the answer to the problem.</p>





```input1
4
1 2
2 3
3 4

```




```input2
5
1 2
2 3
3 4
3 5

```




```input3
8
1 2
2 3
3 4
1 5
5 6
6 7
1 8

```




```output1
8

```




```output2
0

```




```output3
22

```



## Note

<p>In first sample, there are <span class="tex-span">8</span> ways:</p><ul> <li> edge between <span class="tex-span">2</span> and <span class="tex-span">3</span> turns to edge between <span class="tex-span">1</span> and <span class="tex-span">3</span>, </li><li> edge between <span class="tex-span">2</span> and <span class="tex-span">3</span> turns to edge between <span class="tex-span">1</span> and <span class="tex-span">4</span>, </li><li> edge between <span class="tex-span">2</span> and <span class="tex-span">3</span> turns to edge between <span class="tex-span">2</span> and <span class="tex-span">3</span>, </li><li> edge between <span class="tex-span">2</span> and <span class="tex-span">3</span> turns to edge between <span class="tex-span">2</span> and <span class="tex-span">4</span>, </li><li> edge between <span class="tex-span">1</span> and <span class="tex-span">2</span> turns to edge between <span class="tex-span">1</span> and <span class="tex-span">2</span>, </li><li> edge between <span class="tex-span">1</span> and <span class="tex-span">2</span> turns to edge between <span class="tex-span">1</span> and <span class="tex-span">4</span>, </li><li> edge between <span class="tex-span">3</span> and <span class="tex-span">4</span> turns to edge between <span class="tex-span">1</span> and <span class="tex-span">4</span>, </li><li> edge between <span class="tex-span">3</span> and <span class="tex-span">4</span> turns to edge between <span class="tex-span">3</span> and <span class="tex-span">4</span>. <ul></ul></li></ul>
