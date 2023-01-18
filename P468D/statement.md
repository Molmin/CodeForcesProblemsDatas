## Description

<div><p>Little X has a tree consisting of <span class="tex-span"><i>n</i></span> nodes (they are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>). Each edge of the tree has a positive length. Let's define the distance between two nodes <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (we'll denote it <span class="tex-span"><i>d</i>(<i>v</i>, <i>u</i>)</span>) as the sum of the lengths of edges in the shortest path between <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span>. </p><p>A permutation <span class="tex-span"><i>p</i></span> is a sequence of <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. Little X wants to find a permutation <span class="tex-span"><i>p</i></span> such that sum <img align="middle" class="tex-formula" src="file://y0jRXmGY.png" style="max-width: 100.0%;max-height: 100.0%;"> is maximal possible. If there are multiple optimal permutations, he wants to find the lexicographically smallest one. Help him with the task!</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains three space separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤  <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub> ≤  <i>n</i>;&nbsp;1 ≤  <i>w</i><sub class="lower-index"><i>i</i></sub> ≤  10<sup class="upper-index">5</sup>)</span>, denoting an edge between nodes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> with length equal to <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that these edges form a tree.</p></div><div class="output-specification"><p>In the first line print the maximum possible value of the described sum. In the second line print <span class="tex-span"><i>n</i></span> integers, representing the lexicographically smallest permutation.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains three space separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤  <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub> ≤  <i>n</i>;&nbsp;1 ≤  <i>w</i><sub class="lower-index"><i>i</i></sub> ≤  10<sup class="upper-index">5</sup>)</span>, denoting an edge between nodes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> with length equal to <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that these edges form a tree.</p>

## Output

<p>In the first line print the maximum possible value of the described sum. In the second line print <span class="tex-span"><i>n</i></span> integers, representing the lexicographically smallest permutation.</p>





```input1
2
1 2 3

```




```input2
5
1 2 2
1 3 3
2 4 4
2 5 5

```




```output1
6
2 1

```




```output2
32
2 1 4 5 3

```


